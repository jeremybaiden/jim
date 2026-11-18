# Supabase setup for Jim

Project: `auntie-ceci` (ref `kgfijzevpcbcbdrcmszo`, Canada Central), shared with Auntie Ceci. One account works for both apps.

| What | Details |
|---|---|
| Table `jim_items` | One row per saved item (workout, session, custom exercise, settings, body weight, photo record). Columns: `user_id`, `id`, `type`, `data` (jsonb), `updated_at`. Row-level security: each person can only read, add, change and delete their own rows. Rows are deleted automatically if the account is deleted. |
| Bucket `jim-photos` | Private. JPEG/PNG/WebP up to 10 MB. Each person can only upload, view and delete files inside a folder named after their user id. Photos are shown with short-lived signed links. |

## Settings needed in the Supabase dashboard

1. **Authentication → URL Configuration → Redirect URLs**: add `https://jeremybaiden.github.io/jim/` (keep the Auntie Ceci one).
2. **Authentication → Sign In / Providers → Google**: turn on and add the Google OAuth client ID and secret (shared with Auntie Ceci). Until then the Google button shows a message and people can use the email link or continue as guests.

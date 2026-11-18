# Jim · your personal coach

A gym tracker that coaches you: log workouts, weights and reps, and Jim tells you what to lift next time.

**Use it:** https://jeremybaiden.github.io/jim/

## Features

- **Jim (home)**: where you are in the week, today's session with the weights to use, and Jim's notes on what to change.
- **Train**: log sets, reps, weight and reps in reserve, with a rest timer. Sessions start pre-filled with Jim's targets.
- **Plan**: splits for home (no equipment or dumbbells) and commercial gyms, including full body, upper/lower, PPL, Arnold, bro split and sports plans. Weekly sets per muscle against your targets.
- **Progress**: charts and history for any period (last N weeks, a date range, or hand-picked weeks), sets per muscle, strength over time and weekly volume.
- **Exercise library**: 349 exercises from MuscleWiki with main muscles and subgroups (e.g. triceps medial head), multi-select filters, and your own custom exercises.
- **Body weight** tracker with a 7-day average, and private **progress photos** with side-by-side compare.
- **Accounts**: sign in with Google or an emailed link to sync across devices, or use it as a guest (data stays in your browser and moves into your account when you sign in).
- Light and dark mode, phone and desktop layouts, and a demo tour with a sample user.

## How it's built

- `index.html` is the whole app in one file (no build step needed to host it). GitHub Pages serves it from the `main` branch.
- Accounts and saving use Supabase (project `auntie-ceci`, shared with Auntie Ceci). See `supabase/README.md`.

## Copyright

© 2026 Jeremy Baiden. All rights reserved. See [LICENSE](LICENSE).

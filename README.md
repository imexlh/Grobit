# Grobit — Daily Habit Companion

A gentle habit tracker with the original Grobit clover mascot. The garden-building screens have been replaced by a simpler daily companion experience: Home, My Habits, Rewards, Progress, and Profile.

## Supabase setup
1. Open your Supabase project.
2. In **Project Settings → API**, copy the **Project URL** and **anon / publishable key**.
3. Add those two public values to `supabase-config.js`.
4. In **SQL Editor**, run `supabase/schema.sql`.
5. In **Authentication → URL Configuration**, add your Vercel production URL to the allowed Site URL / Redirect URLs.
6. Test sign-up, email confirmation (if enabled), sign-in, progress updates, and sign-out.

## Run locally
`npm install` then `npm run dev`.

## Security and data
- Supabase Auth manages passwords and authentication sessions. Grobit does not save passwords in LocalStorage.
- Habit lists, XP, coins, streaks, and cosmetic rewards are saved in `grobit_profiles.data` as JSONB.
- Row Level Security policies restrict each authenticated user to their own profile row.
- The anon/publishable key is intended for browser use. **Never** put a Supabase `service_role` key or database password in `supabase-config.js` or commit it to GitHub.

## Vercel
The existing Vercel project can deploy this branch as a preview if Git integration is enabled. Merge the branch into `main` only after Supabase configuration and preview testing are complete.

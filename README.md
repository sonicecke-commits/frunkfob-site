# Frunk & Fob: EV gear picks site

Static site for GitHub Pages (Settings > Pages > Deploy from branch `main`, folder `/`).

- `index.html` forwards to `picks/` and keeps `?src=` (2026-11-11: the old fitted-case waitlist page was retired with the affiliate pivot; the last version is commit e3c38a7).
- `picks/index.html` is the EV gear picks page (paid links, tracking ID `frunkfob-20`, budget / mid-range / premium, no prices).
- `picks/kit.js` (same file on all three picks sites) runs the email sign-up and the cookie-free counting:
  - Sign-up posts straight to the MailerLite form "Frunk & Fob site" (account 2745570, form 202515034386990483, double opt-in) with `signup_source` = the `?src=` value.
  - GoatCounter code `frunkfob` counts visits (source = `?src=`), clicks on "See it on Amazon" (`out/<ASIN>`) and sign-ups (`signup`). Nothing is fetched from Amazon.

Bio links: use `?src=instagram`, `?src=tiktok` or `?src=facebook` so visits, clicks and sign-ups show where they came from.

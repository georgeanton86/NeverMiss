# NeverMiss 🎁

**Never forget the people you love.** NeverMiss is a shared-profile app for
occasions, wishlists, and reminders. You build your profile, add the people in
your circle, and everyone's birthdays, anniversaries, and holidays surface as a
single countdown feed — so nobody blanks on a "happy birthday," and nobody
buys the same gift twice.

## What it does

- **Your profile** — your occasions and a wishlist of things you'd love, that
  you can share with family and friends.
- **Your circle** — add the people close to you, grouped into Family / Friends /
  Work, each with their own occasions and wishlist.
- **Countdown feed** — every upcoming occasion across your circle, soonest
  first, with a "days away" countdown and a celebratory hero for the next one.
- **Gift claiming** — quietly claim a gift from someone's wishlist so two people
  don't buy the same thing. The recipient never sees who claimed what.
- **One-tap messages** — occasion-aware message drafts you can tweak and copy,
  so you always have something warm to say.
- **Shareable profile** — a link that shows your occasions and wishlist to the
  people you send it to.

## Run it

It's a single self-contained file — no build step, no install.

```bash
open index.html      # macOS
# or just double-click index.html, or serve the folder:
python3 -m http.server 8000   # then visit http://localhost:8000
```

The app loads React and Tailwind from a CDN and saves your data to the
browser's `localStorage`, seeded with a demo family so it's alive on first open.
There's a **Reset demo** button under the **You** tab.

## Tech & status

Built as a mobile-first prototype: React (UMD) + Tailwind, plain HTML/CSS/JS,
canvas confetti, no backend. Data lives in the browser only.

**Next step to a real product:** a backend with accounts so a circle syncs
across everyone's phones, private invite links, and push/email reminders. The
"smart" layer (nudges like *"order this gift now to arrive in time,"* auto-drafted
messages) sits on top of that foundation.

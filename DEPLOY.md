# Putting NeverMiss on your phone

NeverMiss is now an **installable web app (PWA)**. Once it's online at a real
web address, anyone can add it to their home screen and it behaves like a real
app — its own icon, fullscreen, works offline.

You don't need to code. Pick one path.

---

## Option A — Netlify Drop (easiest, ~3 minutes, free)

1. Download this project folder to your computer (the folder with `index.html`
   in it).
2. Go to **https://app.netlify.com/drop**.
3. **Drag the whole folder** onto the page.
4. Netlify gives you a public HTTPS link like `https://neat-name-123.netlify.app`.
   That's your live app.

**Install it on a phone:**
- **iPhone (Safari):** open the link → tap the **Share** button → **Add to Home
  Screen**.
- **Android (Chrome):** open the link → menu **⋮** → **Install app** / **Add to
  Home Screen**.

You'll get a NeverMiss icon on your home screen that opens fullscreen. 🎉

---

## Option B — GitHub Pages (free, lives with the code)

Since the code is already on GitHub:

1. Merge this branch into `main` (or set Pages to serve this branch).
2. In the repo: **Settings → Pages**.
3. Under **Build and deployment**, set **Source: Deploy from a branch**, pick the
   branch and the `/ (root)` folder, then **Save**.
4. After a minute your app is live at
   `https://<your-username>.github.io/NeverMiss/`.

Install to a phone the same way as above.

---

## What "installed" gets you today

- Home-screen icon and fullscreen, app-like experience.
- Works offline (it caches itself).

## What still needs a backend (the next build)

- **Reminders that reach other people's phones/inboxes** — email digests or push
  notifications sent on a schedule. That requires accounts + a server + a sender.
  See the "Next step" section in `README.md`. The service worker in `sw.js`
  already contains the push-notification handlers, ready for that backend.

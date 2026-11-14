# Stakes (React PWA)
```
npm install
npm run dev        # http://localhost:5173
npm run build && npm run preview   # production build, service worker + install prompt active
```
- `public/manifest.json` makes it installable (Add to Home Screen / Install app). It needs HTTPS in production (localhost is fine).
- `public/sw.js` caches the app shell so it opens offline. It only registers in production builds.
- Icons are in `public/icons/`; the logo component is `src/Logo.jsx`.
- Deploy `dist/` to Vercel, Netlify or Cloudflare Pages (set the SPA fallback to `/index.html`).

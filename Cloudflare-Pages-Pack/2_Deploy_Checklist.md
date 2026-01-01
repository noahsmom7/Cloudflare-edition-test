# Deploy Checklist (copy/paste safe)

## If you have a built folder (dist/build)
1. Put everything from your `dist/` (or `build/`) into: `direct-upload/PLACE_YOUR_DIST_HERE/`
2. Keep `_redirects` and `_headers` at the ZIP root.
3. Cloudflare → Workers & Pages → Create application → Pages → **Use direct upload**
4. Drag **all files from ZIP root** (not the folder itself).
5. Deploy → your site appears at `https://<project>.pages.dev`

## If you have full source (Vite/CRA)
1. Ensure `package.json` has `"build": "vite build"` (Vite) or CRA build.
2. Push repo to GitHub.
3. Cloudflare Pages → Create Project → **Connect Git** → pick repo.
4. Preset **Vite** or **Create React App**; Build: `npm run build`; Output: `dist` (Vite) or `build` (CRA).
5. Deploy.

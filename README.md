# LumaCraft Legal Pages

Public static site for LumaCraft Studio legal and support pages.

## Structure

- `public/index.html`
- `public/support.html`
- `public/privacy.html`
- `public/terms.html`
- `public/app-ads.txt`
- `firebase.json`
- `.firebaserc.example`
- `public/LumaFocus/index.html`
- `public/LumaFocus/privacy.html`
- `public/LumaFocus/terms.html`

## Publication values

- Support email: `lumacraftstudio.support@gmail.com`
- Legal / display name: `LumaCraft Studio`
- LumaFocus effective date: `April 19, 2026`

## Current publication target

Primary production target is the custom domain:

- `https://lumacraftstudio.in/`
- `https://lumacraftstudio.in/privacy`
- `https://lumacraftstudio.in/terms`
- `https://lumacraftstudio.in/support`
- `https://lumacraftstudio.in/app-ads.txt`
- `https://lumacraftstudio.in/LumaFocus/`

Current Firebase Hosting staging baseline:

- Firebase project id: `lumacraft-studio-46d50`
- Temporary Hosting URL: `https://lumacraft-studio-46d50.web.app`
- Current deploy command:
  - `npx firebase deploy --only hosting`
- Current publish root:
  - `public/`

## Legacy GitHub Pages URLs

If this repo is published as `lumacraft-legal` under the `krishnasharmabsr` account, the Pages URLs will typically be:

- Legacy video editor privacy policy:
  `https://krishnasharmabsr.github.io/lumacraft-legal/privacy.html`
- Legacy video editor terms:
  `https://krishnasharmabsr.github.io/lumacraft-legal/terms.html`
- LumaFocus legal home:
  `https://krishnasharmabsr.github.io/lumacraft-legal/LumaFocus/`
- LumaFocus privacy policy:
  `https://krishnasharmabsr.github.io/lumacraft-legal/LumaFocus/privacy.html`
- LumaFocus terms:
  `https://krishnasharmabsr.github.io/lumacraft-legal/LumaFocus/terms.html`

## Notes

- Keep this repository public.
- Preserve root-level hosted URLs `/privacy` and `/terms` for backward compatibility.
- New apps should be added as subpaths rather than separate branches.
- `app-ads.txt` must stay at the domain root for AdMob verification.
- Replace `pub-REPLACE_WITH_YOUR_ADMOB_PUBLISHER_ID` in `app-ads.txt` with the real AdMob publisher ID before deployment.
- Copy `.firebaserc.example` to `.firebaserc` and replace the Firebase project id before running Firebase Hosting deploys.
- Do not commit `.firebaserc`, `.firebase/`, access tokens, service-account keys, or registrar credentials.
- Only public/support-facing values belong in this repo:
  - legal pages
  - support contact email
  - public domain URLs
  - public `app-ads.txt` seller line

## Remaining production steps

1. Add custom domain `lumacraftstudio.in` in Firebase Hosting.
2. Copy Firebase-provided DNS records into Hostinger.
3. Wait for domain verification and SSL provisioning.
4. Verify:
   - `https://lumacraftstudio.in/`
   - `https://lumacraftstudio.in/privacy`
   - `https://lumacraftstudio.in/support`
   - `https://lumacraftstudio.in/app-ads.txt`
5. Update the Play Console developer website to `https://lumacraftstudio.in`.
6. Wait for AdMob to crawl and verify `app-ads.txt`.

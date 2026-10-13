# mutatis-site

Public site for mutatismacro.com, served by GitHub Pages. This repo holds only
published output; the models and code live in the private `transmission` repo.

## Current content
A holding page (`index.html`) with the product pitch, an interactive
illustration of the method, and a newsletter sign-up.

## Publish the holding page
1. Create a **public** GitHub repo named `mutatis-site` and push this folder to `main`.
2. Repo → Settings → Pages → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Custom domain `mutatismacro.com` (the `CNAME` file already sets it), DNS per
   `transmission/docs/DEPLOYMENT.md`, then tick **Enforce HTTPS**.

When the Quarto site is ready, the publisher agent switches Pages to the
`gh-pages` branch per DEPLOYMENT.md and this holding page is replaced.

## Newsletter sign-up
The form posts to Buttondown. Create an account, then set
`const BUTTONDOWN_USER = "<your username>";` near the bottom of `index.html`.
Until then the form validates the address and says sign-ups open shortly.

## Privacy
No analytics, cookies or trackers. Fonts load from Google Fonts.

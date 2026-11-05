# Uncut Me — Netlify deployment package

This is a prebuilt static website. It does not need a build command or external dependencies.

## Fastest option: manual upload

1. Sign in to Netlify and open <https://app.netlify.com/drop>.
2. Drag the `site` folder onto the deploy area.
3. Netlify will publish it and provide a temporary `netlify.app` address.
4. Use **Customize** in Netlify if you want to rename the address or connect a custom domain.

The `uncut-me-netlify-upload.zip` archive contains the same deployable files with `index.html` at its root. If Netlify asks for a folder rather than an archive, unzip it first and drag the extracted folder.

## Git-based deployment

The source is maintained at <https://github.com/osvaldojrp/bruno> on the `master` branch. Import that repository into Netlify for automatic deployments after each push. The included `netlify.toml` sets `site` as the publish directory, with no build command required.

## Project address

The package is configured for `https://uncut-me-autobiography.netlify.app/` in its canonical, social-sharing, sitemap and robots metadata. If you later connect a custom domain, update those absolute URLs to the custom-domain address.

## Amazon book links

Kindle and paperback buttons are managed centrally in `site/site-config.js`. The Kindle button uses the live Amazon product page. The paperback URL remains an Amazon search placeholder until the physical-book listing is ready. Replacing the relevant value updates every matching button across the site automatically.

Verify `/` and `/about.html` after deployment. The shorter `/about` path is also supported.

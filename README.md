# Glaze Keeper website

A responsive static website for Glaze Keeper. No build step, JavaScript, analytics, remote fonts, or dependencies. The privacy policy is readable without scripts or sign-in.

## Structure

- `index.html`: minimal app introduction.
- `privacy/index.html`: privacy policy at the stable `/privacy/index.html` path.
- `assets/styles.css`: shared colors, typography, mobile layout, and print styles.
- `.nojekyll`: serves files directly on GitHub Pages.

## Before publication

Confirm the policy against the actual submitted release, its bundled SDKs, and support email practices. The draft reflects the app source and privacy audit as of September 25, 2026; it is not a production-binary/network audit. Confirm the correspondence retention and service-provider commitments, and revise the date when finalizing. Public contact: Kyle Swensson, kyle.swensson.bis@gmail.com.

Apple also requires an easily accessible privacy policy link inside the app. Once the site is live, add the URL below to Settings → About. The app's author credit has been updated, but the privacy link remains a release task. Keep App Store Connect’s App Privacy answers consistent with the released app. A public policy alone does not complete submission. Apple also requires a working support URL with current contact information; add support content before using this site for that separate field.

## Publish on GitHub Pages

Repository: https://github.com/KyleSwensson/GlazeKeeperWebsite

1. Commit and push the website files to `main` after reviewing the policy.
2. In GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**, then **main** and **/ (root)**. Save.
4. Enable **Enforce HTTPS** when available. Wait for deployment, then use **Visit site** to confirm the address. GitHub Free requires a public repository for Pages.
5. Open both pages in a signed-out browser and check navigation and the contact email.

Expected homepage: https://kyleswensson.github.io/GlazeKeeperWebsite/

Expected App Store Connect Privacy Policy URL: **https://kyleswensson.github.io/GlazeKeeperWebsite/privacy/index.html**

These are expected addresses, not confirmation that the site is live. Enter the working HTTPS privacy URL in App Store Connect’s App Privacy section and use that same address in the app.

## Preview and extend

Open `index.html` or `privacy/index.html` directly in a browser for a quick preview. For an HTTP preview, serve this directory with any static file server.

Add future pages as `page-name/index.html`, link their stylesheet with `../assets/styles.css`, and reuse the semantic header/footer. Add navigation links to each page, pointing explicitly to its index.html file so links also work when opened directly from disk. Relative internal links work under GitHub Pages’ repository subdirectory and a future custom domain. Keep `/privacy/index.html` stable when expanding or migrating the site. Shared CSS variables provide the app’s cream, green, and clay palette.

## References

- [Apple App Review Guidelines, section 5.1.1](https://developer.apple.com/app-store/review/guidelines/#data-collection-and-storage): policy links in App Store Connect and the app; data use, sharing, retention, deletion, and consent choices.
- [Manage App Privacy](https://developer.apple.com/help/app-store-connect/manage-app-information/manage-app-privacy)
- [Create a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)
- [GitHub General Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement)

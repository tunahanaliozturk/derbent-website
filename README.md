# derbent-website

The website of [Derbent](https://github.com/tunahanaliozturk/derbent): the landing page, the user
documentation and the release notes. Built with Docusaurus and deployed to GitHub Pages by the `website`
workflow on every push to `main`.

```bash
npm ci
npm start          # http://localhost:3000, reloads on change
npm run build      # the production build in build/, fails on broken links
```

- Docs: `docs/`, sidebar in `sidebars.js`
- Release notes: `releases/`; a note with `draft: true` stays off the published site
- Landing page: `src/pages/index.js`
- Logo and favicon: `static/`

The workflow reads the site's origin and base path from the repository's Pages settings, so setting a
custom domain there needs no change in the code.

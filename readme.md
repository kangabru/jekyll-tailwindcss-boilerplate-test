# Jekyll & Tailwind CSS Boilerplate

A bare bones [Jekyll](https://jekyllrb.com/) site which comes preconfigured to use [Tailwind CSS](https://tailwindcss.com/) for styling.

> 👉 [Try the demo here](https://jekyll-tailwindcss-boilerplate.netlify.app/).

## Features

- 🤍 Ships free of styling or theming. [Add a theme](https://jekyllrb.com/resources/) or [get started with Tailwind CSS](https://tailwindcss.com/docs/utility-first/).
- 📈 Ships Google Analytics and SEO ready
- 🍕 Dev mode: your Jekyll site is refreshed on file changes and all Tailwind CSS classes are available for use.
- 💻 Release mode: CSS is optimised by striping out unused classes and minifying the file.

---

## 👟 Install

Ensure [Ruby](https://www.ruby-lang.org/en/downloads/) and [npm](https://www.npmjs.com/get-npm) are installed then setup the project:
```
npm run setup
```

## 🍕 Develop

```
npm start
```
Parcel and Jekyll will run concurrently so file changes update automatically.

## 💻 Release

```
npm run rel
```
Tailwind CSS is minified and Jekyll outputs the site to the `_site` folder.

Deploy statically (e.g. [Netlify](https://www.netlify.com/)) with the following build settings:
- Command: `npm run build`
- Directory: `_site`

---

## 🤔 Troubleshoot

### My styling disappears when deployed
-  Jekyll markdown may generate elements that are being purged by Tailwind CSS. [See these docs](https://tailwindcss.com/docs/optimizing-for-production#purge-css-options) to whitelist elements or configure PurgeCSS further.
- Don't build up class names like `"my" + "-class"`. Use full names like `"my-class"` instead.
- Don't whitelist the `_site/` folder as this folder is not guaranteed to exist when deployed to a server.

### Have another issue?
Contact me by posting an issue. I'll be happy to help 🙂

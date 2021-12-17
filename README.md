# @gorrion/prettier-config

Prettier config used at Gorrion Software House

## Usage

Install the package using `npm` (or `yarn` or `pnpm`)

```
npm install --save-dev @gorrion/prettier-config
```

Add the `prettier` key to your `package.json`

```diff
diff --git a/package.json b/package.json
--- a/package.json
+++ b/package.json
   "keywords": [
     "prettier"
   ],
+  "prettier": "@gorrion/prettier-config",
   "author": {
    "name": "Gorrion Software House",
    "url": "https://gorrion.io"
  },
  "main": "index.js"
```

## Overwrite

If you need to overwrite some settings, create `.prettierrc.js` file, import config and export modifications, e.g:

```js
module.exports = {
  ...require("@gorrion/prettier-config"),
  semi: false,
};
```

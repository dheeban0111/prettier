Prettier v3 will change the plugin's interface.
So this document describes how to migrate to v3 for plugin developers.

## 1.
Remove use of `prettier.doc.build.concat()`, use array literal instead.

- **Don't forget to update logic if your plugin traverse docs.**

https://github.com/prettier/prettier/blob/next/changelog_unreleased/api/13203.md

## 2.
Remove 2nd parameter in `parse()` function.
If you need core plugins check how to get the core plugins from the changelog.

- **`parse()` can be async function**

https://github.com/prettier/prettier/blob/next/changelog_unreleased/api/13268.md

## 3.
Update `embed()` function.

Check [this link](https://deploy-preview-9583--prettier.netlify.app/docs/en/next/plugins.html#optional-embed) to see how the new `embed` works.

- **If your plugin doesn't support `embed()` print, make sure you remove it (Empty function will cause print process slower).**
- **If your plugin supports `embed()` print and you already have `visitorKeys` for your AST, please add [`getVisitorKeys()` function](https://deploy-preview-9583--prettier.netlify.app/docs/en/next/plugins.html#optional-getvisitorkeys), it will improve `embed()` print.**
- **If your plugin supports `embed()` print and your AST have cycles, make sure exclude them in [`getVisitorKeys()` function](https://deploy-preview-9583--prettier.netlify.app/docs/en/next/plugins.html#optional-getvisitorkeys), otherwise your plugin won't work.**

## 4.
If you are calling Prettier APIs inside your plugin or tests, make sure they are `await`ed.
https://github.com/prettier/prettier/blob/next/changelog_unreleased/api/12574.md


## 5.
You can migrate your plugin to ES Module if you like.
https://github.com/prettier/prettier/blob/next/changelog_unreleased/api/13201.md
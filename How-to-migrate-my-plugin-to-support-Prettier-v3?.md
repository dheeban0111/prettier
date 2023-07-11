Prettier v3 will change the plugin's interface.
So this document describes how to migrate to v3 for plugin developers.

## 1. Remove use of `prettier.doc.build.concat()`, use array literal instead.

Notes:

- **Don't forget to update logic if your plugin traverse docs.**

[Changelog](https://prettier.io/blog/2023/07/05/3.0.0.html#update-prettierdoc-13203httpsgithubcomprettierprettierpull13203-14456httpsgithubcomprettierprettierpull14456-by-fiskerhttpsgithubcomfisker)

## 2. Remove 2nd parameter in `parse()` function.

If you need core plugins check how to get the core plugins from [the changelog](https://prettier.io/blog/2023/07/05/3.0.0.html#the-second-argument-parsers-passed-to-parsersparse-has-been-removed-13268httpsgithubcomprettierprettierpull13268-by-fiskerhttpsgithubcomfisker).

Notes:

- **`parse()` can be async function**

[Changelog](https://prettier.io/blog/2023/07/05/3.0.0.html#the-second-argument-parsers-passed-to-parsersparse-has-been-removed-13268httpsgithubcomprettierprettierpull13268-by-fiskerhttpsgithubcomfisker)

## 3. Update `embed()` function.

Check [this link](https://prettier.io/docs/en/plugins.html#optional-embed) to see how the new `embed` works.

Notes:

- **If your plugin doesn't support `embed()` print, make sure you remove it (Empty function will cause print process slower).**
- **If your plugin supports `embed()` print and you already have `visitorKeys` for your AST, please add [`getVisitorKeys()` function](https://prettier.io/docs/en/plugins.html#optional-getvisitorkeys), it will improve `embed()` print.**
- **If your plugin supports `embed()` print and your AST have cycles, make sure exclude them in [`getVisitorKeys()` function](https://prettier.io/docs/en/plugins.html#optional-getvisitorkeys), otherwise your plugin won't work.**

## 4. `await` your Prettier API calls.

If you are calling Prettier APIs inside your plugin or tests, make sure they are `await`ed.

[Changelog](https://prettier.io/blog/2023/07/05/3.0.0.html#change-public-apis-to-asynchronous-12574httpsgithubcomprettierprettierpull12574-12788httpsgithubcomprettierprettierpull12788-12790httpsgithubcomprettierprettierpull12790-13265httpsgithubcomprettierprettierpull13265-by-fiskerhttpsgithubcomfisker)


## 5. (optional) You can migrate your plugin to ES Module if you like.

[Changelog](https://prettier.io/blog/2023/07/05/3.0.0.html#support-plugins-in-esm-13201httpsgithubcomprettierprettierpull13201-by-fiskerhttpsgithubcomfisker)
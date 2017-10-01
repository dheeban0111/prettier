**[List of active labels](https://github.com/prettier/prettier/labels?sort=name-asc)**

Issue labels fall into the following groups.

## Area

Areas are parts of the code-base that frequently have issues.

* <kbd>area:comments</kbd>
  
  Comments are one of the most complicated parts of prettier. This label means the issue relates to how prettier is printing comments.

## Difficulty

Difficulty is used to mark how much time it will likely take to resolve an issue, or how much nuance there is to a particular issue. 

* <kbd>difficulty:easy</kbd>

  This issue is easy. Resolve me on the train to work!

* <kbd>difficulty:hard</kbd>

  This issue might take an entire weekend, or require a tough decision.

## Language

Prettier supports a growing number of languages so it is useful to tag them.

* <kbd>lang:css/scss/less</kbd>

  This issue affects CSS, LESS or SCSS.

* <kbd>lang:flow</kbd>

  This issue affects Flow.

* <kbd>lang:graphql</kbd>

  This issue affects GraphQL.

* <kbd>lang:jsx</kbd>

  This issue affects JSX.

* <kbd>lang:javascript</kbd>

  This issue affects JavaScript.

* <kbd>lang:typescript</kbd>

  This issue affects TypeScript.

## Priority

* <kbd>priority:high</kbd>

  High priority issues are ones that either re-print code in a way that unintentionally changes the AST, or are significant regressions and need to be fixed urgently.

* <kbd>priority:facebook blocker</kbd>

  Facebook use Prettier internally. Issues marked with this label block Facebook upgrading Prettier.

## Scope

* <kbd>scope:dependency</kbd>

  This is a real issue but cannot be solved by modifying Prettier itself, it must be fixed in one of our dependencies.

* <kbd>scope:external</kbd>

  This issue cannot be resolved in Prettier itself, it is an issue with something external, such as an editor integration.


## Status

Status labels are particularly useful for finding issues that need attention.

* <kbd>status:awaiting response</kbd>

  In a pull request, this means a review has been left that requires the author to reply. On an issue, this means that a collaborator has replied and requires more information from the reporter to proceed.

* <kbd>status:has pr</kbd>

  This issue has an accompanying PR. By excluding this label from your search it is easier to find actionable items.

* <kbd>status:help wanted</kbd>

  Help! We're only a small group of collaborators who unfortunately can't get to every issue promptly. This label means we think the issue should be addressed but don't have the capacity to resolve it now. Great for first-time contributors!

* <kbd>status:needs discussion</kbd>

  This issue needs discussion and ultimately a decision to be made before it is actionable.

## Type

Issue types are categories that an issue might fall into. Generally an issue should have exactly one type.

* <kbd>type:bug</kbd>

  Red alert! Issues with this label are bugs in Prettier. Most bugs are cases where Prettier does not produce the expected output. If the output means the code can no-longer be parsed, or the meaning of the code has changed, add the <kbd>priority:high</kbd> label, too. 

* <kbd>type:docs</kbd>

  This issue requires amending or adding new documentation.


* <kbd>type:duplicate</kbd>

  This issue is a duplicate of a previous issue.

* <kbd>type:editor support</kbd>

  This issue pertains to ensuring Prettier provides the right tools to be used inside editor integrations.

* <kbd>type:feature</kbd>

  Working as intended! Issues with this label represent a potential new feature to be added to prettier.

* <kbd>type:infrastructure/meta</kbd>

  This issue is about CI, publishing to npm, the status of Prettier, or anything else about Prettier itself.

* <kbd>type:option request</kbd>

  Prettier gets a lot of requests to add options to change the way it will print some code. Because Prettier is opinionated, and due to the cost of maintaining options, we will often refuse to add them. [Read this](https://github.com/prettier/prettier/issues/40) for more context.

* <kbd>type:question</kbd>

  Issues marked as questions are queries about how prettier works, or bug reports that are actually prettier working as intended.


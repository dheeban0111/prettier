**[List of active labels](https://github.com/prettier/prettier/labels?sort=name-asc)**

Issue labels fall into the following groups.

## Area

Areas are parts of the code-base.

* <kbd>area:api</kbd>
  
  Issues about Prettier's Application Programming Interface.

* <kbd>area:cli</kbd>
  
  Issues about Prettier's Command Line Interface.


* <kbd>area:tests</kbd>
  
  Issues about Prettier's tests and test infrastructure.

* <kbd>area:comments</kbd>
  
  Comments are one of the most complicated parts of prettier. This label means the issue relates to how prettier is printing comments.

* <kbd>area:multiparser</kbd>
  
  Multi-parser is the code that makes it possible to format one programming language inside another, such as CSS-in-JS.

* <kbd>area:playground</kbd>
  
  Issues about the [playground](https://prettier.io/playground/).

* <kbd>area:website</kbd>
  
  Issues about the [website](https://prettier.io/), excluding playground.

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

* <kbd>lang:javascript</kbd>

  This issue affects JavaScript.

* <kbd>lang:json</kbd>

  This issue affects JSON.

* <kbd>lang:jsx</kbd>

  This issue affects JSX.

* <kbd>lang:markdown</kbd>

  This issue affects Markdown.

* <kbd>lang:typescript</kbd>

  This issue affects TypeScript.

* <kbd>lang:handlebars</kbd>

  This issue affects Handlebars.

## Priority

* <kbd>priority:facebook blocker</kbd>

  Although Prettier is not an official project of Facebook OpenSource, engineers working at Facebook (primarily @vjeux) have devoted a significant number of working hours to improving Prettier for everybody. Facebook use Prettier internally, and issues marked with this label block Facebook upgrading Prettier.

* <kbd>priority:high</kbd>

  High priority issues are ones that either re-print code in a way that unintentionally changes the AST, or are significant regressions and need to be fixed urgently.

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

* <kbd>help wanted</kbd>

  Help! We're only a small group of collaborators who unfortunately can't get to every issue promptly. This label means we think the issue should be addressed but don't have the capacity to resolve it now. Great for first-time contributors!

* <kbd>status:needs discussion</kbd>

  This issue needs discussion and ultimately a decision to be made before it is actionable.

* <kbd>status:wip</kbd>

  In a pull request, marks that the code changes are a work in progress and should not be merged.

## Type

Issue types are categories that an issue might fall into. Generally an issue should have exactly one type.

Want to triage some issues? [This query](https://github.com/prettier/prettier/issues?utf8=%E2%9C%93&q=is%3Aissue%20is%3Aopen%20-label%3Atype%3Abug%20-label%3Atype%3Aenhancement%20-label%3Atype%3Aquestion%20-label%3A%22type%3Aoption%20request%22%20-label%3Atype%3Adocs%20-label%3A%22type%3Aeditor%20support%22%20-label%3Atype%3Ainfra%20-label%3Atype%3Ameta%20-label%3Atype%3Aduplicate%20-label%3Atype%3Atests) lists all open issues without a type label.

* <kbd>type:bug</kbd>

  Red alert! Issues with this label are bugs in Prettier. Most bugs are cases where Prettier does not produce the expected output. If the output means the code can no-longer be parsed, or the meaning of the code has changed, add the <kbd>priority:high</kbd> label, too. 

* <kbd>type:docs</kbd>

  This issue requires amending or adding new documentation.

* <kbd>type:duplicate</kbd>

  This issue is a duplicate of a previous issue.

* <kbd>type:editor support</kbd>

  This issue pertains to ensuring Prettier provides the right tools to be used inside editor integrations.

* <kbd>type:enhancement</kbd>

  Working as intended! Issues with this label represent a potential new feature to be added to Prettier.

* <kbd>type:infra</kbd>

  This issue is about CI, publishing to npm, or similar.

* <kbd>type:intended</kbd>

  Bug reports that are actually prettier working as intended.

* <kbd>type:meta</kbd>

  The status of Prettier, or anything else about Prettier itself.

* <kbd>type:option request</kbd>

  Prettier gets a lot of requests to add options to change the way it will print some code. Because Prettier is opinionated, and due to the cost of maintaining options, we will often refuse to add them. [Read this](https://github.com/prettier/prettier/issues/40) for more context.

* <kbd>type:question</kbd>

  Questions and support requests. Issues marked as questions are automatically closed by a [bot](https://github.com/dessant/support-requests) suggesting to use Stack Overflow instead. The issue tracker is only for development.

* <kbd>type:tests</kbd>

  Tests that are not correct, suggestions for tests that should be added, or similar.

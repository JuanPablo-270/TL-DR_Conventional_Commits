## Commit Messages

### Commit Types

| Type     | Description                                   |
| -------- | --------------------------------------------- |
| build    | build system or external dependencies changes |
| ci       | CI configurations and scripts changes         |
| docs     | documentation                                 |
| feat     | feature                                       |
| fix      | bug fix                                       |
| perf     | improves performance                          |
| refactor | neither fixes a bug or adds a feature         |
| revert   | reverts a previous commit                     |
| styles   | formatting, missing semi colons, etc.         |
| test     | adding missing tests                          |

### Scope
- Could be anything specifying place of the commit change. For example $location, $browser, $compile, $rootScope, ngHref, ngClick, ngView, etc...
### Subject
- Use imperative, present tense: "change" not “changed” nor “changes”
- Don't capitalize first letter - no dot (.) at the end
### Body

- Use imperative, present tense: “change” not “changed” nor “changes”
- Includes motivation for the change and contrasts with previous behavior
### Footer
- Contain any information about breaking changes with the description of the change, justification and migration notes
- Reference GitHub issues that this commit Closes. such as closed bugs should be listed in the footer prefixed with "Closes" keyword like: "Closes #234, #241"
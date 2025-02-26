
**Conventional Commits: A Guide for Consistent Git History**

**What are Conventional Commits?**

Conventional Commits are a specification that provides an easy set of rules for creating an explicit commit history. This makes it easier to automate tools, understand changes, and improve collaboration.

**Why Use Conventional Commits?**

* **Automated Changelogs:** Generate changelogs automatically.
* **Semantic Versioning:** Determine semantic version bumps automatically.
* **Clear History:** Make your Git history more readable.
* **Improved Collaboration:** Provide a common language for teams.

**The Conventional Commits Specification**

A commit message structured according to the Conventional Commits specification must be formatted as follows:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

**Elements of the Commit Message:**

* **`<type>`:**
    * `feat`: A new feature.
    * `fix`: A bug fix.
    * `docs`: Documentation changes.
    * `style`: Changes that do not affect the meaning of the code (formatting, white-space, etc.).
    * `refactor`: A code change that neither fixes a bug nor adds a feature.
    * `perf`: A code change that improves performance.
    * `test`: Adding missing tests or correcting existing tests.
    * `build`: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm).
    * `ci`: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs).
    * `chore`: Other changes that don't modify src or test files.
    * `revert`: Reverts a previous commit.
* **`[optional scope]`:**
    * A scope may be provided to a commit's type, to provide additional contextual information and is contained within parenthesis, e.g., `feat(users): add login`.
* **`<description>`:**
    * A short description of the change.
    * Use the imperative, present tense: "add feature" not "added feature".
* **`[optional body]`:**
    * A longer description of the change.
    * Provides context and reasoning.
    * Use the imperative, present tense.
* **`[optional footer(s)]`:**
    * Information about Breaking Changes (`BREAKING CHANGE:`) or issue references.
    * `BREAKING CHANGE:` should be placed at the beginning of the footer section.
    * Issue references, like closing issues, example: `Closes #123`, `Fixes #456`.

**Examples**

* **Simple fix commit:**

```
fix: correct minor typos in code

see the issue for details on the typos fixed.

closes #12
```

* **Commit with scope:**

```
feat(auth): add user authentication

Implement user login and registration features.
```

* **Breaking change commit:**

```
feat(api): introduce new API endpoint

BREAKING CHANGE: The previous API endpoint has been removed.
```

**Practical Tips**

* **Use a Git client or extension:** Some Git clients and IDE extensions support Conventional Commits, providing helpful prompts.
* **Consistency is key:** Ensure your team follows the same conventions.
* **Automate checks:** Use tools to validate commit messages.
* **Integrate with CI/CD:** Automate changelog generation and versioning in your CI/CD pipeline.
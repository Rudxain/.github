# Intro
Don't be shy! All my repos are open to suggestions and contributions.

# Opening Issues
1. Please search for duplicates. I don't like redundancy.
2. Issues can be used to ask support questions, and feature requests, not just bugs.
3. Use [**Discussions**](https://resources.github.com/devops/process/planning/discussions) instead of Issues when appropriate. Think of Discussions as *subreddits*.

# Opening Pull Requests
- Note: "PR" may also mean "Public Repo".
1. It's recommended to open an issue before a PR, to be sure that your PR will be accepted. If you're confident that your PR doesn't need confirmation, then just do it!
2. Explain **why** your PR makes some changes. A *"why"* is more meaningful than a *"what"*.
3. Any diff sizes are accepted, but small PRs are preferred because they're easier and faster to review. Big PRs are *dreams and nightmares* **simultaneously**.
4. Write "Closes #n" or "Fixes #n" (`n` is the ID) in the main description of the PR to auto-close corresponding issues. This is helpful because it links Issues with PRs for easier navigation.

## Style & Formatting of code
1. **ALWAYS USE TABS** FOR INDENTATION. [This article explains better than me](https://dev.to/alexandersandberg/why-we-should-default-to-tabs-instead-of-spaces-for-an-accessible-first-environment-101f).
2. Use single quotes (') because they look cleaner. Use double quotes (") if compression ratio is a concern (like HTML files served over HTTP with auto-GZip enabled). This rule doesn't apply to Rust.
3. Manual formatting is preferred, because I personally think that [_programming is an art_](https://en.wikipedia.org/wiki/The_Art_of_Computer_Programming), and it's better if it has a "human touch". However, occasional use of formatters like [`rustfmt`](https://github.com/rust-lang/rustfmt), [StandardJS](https://standardjs.com), or [Python Black](https://pypi.org/project/black), are allowed.
4. Reduce semicolons (;) to the bare minimum. Unless it helps with clarity and disambiguation.
5. In case of doubt, search for patterns in the way the code is written, and try to replicate those patterns, for consistency.

# Etc
Most of my repos use [Semantic Versioning](https://semver.org).

If you don't understand something, make sure to read source-code comments and documentation files (like this one)

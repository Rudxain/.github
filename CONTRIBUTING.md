# Contribution Guidelines

Don't be shy! All my repos are open to contributions and suggestions (even style/format requests)

## Issues & Pull Requests

- Avoid opening duplicates, reuse existing ones if those are related
- Any PR diff-size is accepted, but small PRs are preferred because they're easier/faster to review. Big PRs are *dreams and nightmares* **simultaneously**

## Style & Formatting

- [One of the reasons why I prefer tabs over spaces](https://dev.to/alexandersandberg/why-we-should-default-to-tabs-instead-of-spaces-for-an-accessible-first-environment-101f)
- Use -1 (relative, clamped to 0) level of indent in JSON. This is to reduce redundancy. Example:
```json
{
	"❌": "no"
}
{
"✅": "ok"
}
```
- If you type a subjective comment, surround it within quotes, and include your name (any: display-name, username, etc...). Example:
```py
# "I couldn't find a better alternative" @ghost
```
This is to avoid confusion (for future readers) caused by *unintentional impersonation*. This way, everyone knows who said what, without reading the git-blame. Objective comments (like `# this X implementation is faster than Y`) don't need usernames
- Use spaced comments for non-code. Examples:
```py
# ✅
#❌
#0 + 0 # ✅
# 0 + 0 #❌
```
- In case of doubt, search for patterns in the way the code is written, and please try to replicate those patterns, for consistency

## etc

- I'm slowly switching to Rust (maybe even Zig? 👀) and TypeScript, so I'm manually transpiling from JS.
I would appreciate if you helped me convert my repos :)
- I'm not supporting corp-specific HTML (looking at you, Apple-icons and Twitter-cards). Open-Graph already solves this, even though it was created by Meta

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
- Use minimal asterisks in JSDoc. Example:
```js
/**
 * ❌no
*/
/**
✅ok
*/
```
- If you type a subjective comment, surround it within quotes, and include your name (any: display-name, username, user ID, etc...). Example:
```py
# "I couldn't find a better alternative" @ghost
```
This is to avoid confusion (for future readers) caused by *unintentional impersonation*. This way, everyone knows who said what, without reading the git-blame. Objective comments (like `# this X implementation is faster than Y`) don't need usernames
- If a comment needs 3 or more lines, it must be a block-type not line-type. This is to reduce redundant "//". This rule doesn't apply to Rust nor Go, because "idiomatic"
- Use spaced comments for non-code. Examples:
```js
// ok
//no
//0 + 0 // ok
```
```py
# 0 + 0 #no
```
- In case of doubt, search for patterns in the way the code is written, and please try to replicate those patterns, for consistency

## etc

- I'm slowly switching to Rust and Python, so I'm manually transpiling from JS.
I would appreciate if you helped me convert my repos :)
- I'm not supporting Apple's non-standard HTML icons, they must adhere to web-stds
- I'm not supporting HTML Twitter-Cards. Open-Graph already solves this

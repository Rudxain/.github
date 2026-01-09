# Contribution Guidelines

Don't be shy! Most of my repos are open to contribs and suggestions (even style/format requests)

I assume you've (mostly) read these:
- [Learn Git](https://git-scm.com/learn)
- [Basic GH docs](https://docs.github.com/en/get-started)

For anything not specified here, use [common-sense](https://en.wikipedia.org/wiki/Common_sense) and follow "best practices"

## Issues & Pull Requests

- Any PR patch-size is fine, but small PRs are preferred because they're easier/faster to review. Big PRs are *dreams and nightmares* **simultaneously**
- I prefer rebasing rather than merging. [Update your PR branch](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/keeping-your-pull-request-in-sync-with-the-base-branch) by rebasing. Only `merge` if there's a complicated merge-conflict.
> [!tip]
> You can update with Git (CLI) alone, but your local repo must have both remotes. Example:
> ```sh
> git fetch upstream && \
> git rebase upstream/main && \
> git push --force-with-lease
> ```
> Or you can update the remote before your local branch:
> ```sh
> gh pr update-branch --rebase && \
> git pull -r
> ```
- If your PR has too many commits, I'll be tempted to `squash` it. If you keep the `log` tidy, then I'll try to preserve your commits.
- If my review requested changes, I suggest [converting to draft](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/changing-the-stage-of-a-pull-request) while you're applying them, then mark as "ready" after `push`ing. This way, you can notify me without commenting.

## Style & Formatting

- Why I prefer tabs over spaces
	- [Alexander Sandberg advocates for accesibility](https://dev.to/alexandersandberg/why-we-should-default-to-tabs-instead-of-spaces-for-an-accessible-first-environment-101f)
	- [Lea Verou outlines several reasons](https://lea.verou.me/blog/2012/01/why-tabs-are-clearly-superior)
- Please use -1 (relative, clamped to 0) level of indent in JSON. This is to reduce redundancy. Example:
```json
{
	"❌": "no"
}
{
"✅": "ok"
}
```
That rule only applies if the entire file is just 1 object (array or dictionary, nested or flat). IOW, [JSONL](https://jsonlines.org/) is exempt, for better readability. These rules also extrapolate to Lua-Table-Notation (LTN or ["LON"](https://github.com/rmuch/liblon)), and any other format where there's a "base level" of indentation.
- If you add a subjective comment, surround it within quotes, and include your name (any: display-name, username, etc...). Example:
```sh
# "I couldn't find a better alternative" @ghost
```
This is to avoid confusion (for future readers) caused by *unintentional impersonation*. This way, everyone knows who said what, without `git blame`. Objective comments (like `# this X implementation is faster than Y`) don't need usernames
- [Use spaced comments for non-code](https://github.com/helix-editor/helix/issues/14516). Examples:
```sh
# ✅
#❌
#0 + 0 # ✅
# 0 + 0 #❌
```
- In case of doubt, search for patterns in the way the code is written, and please try to replicate those patterns, for consistency
- Read [my `.files`](https://github.com/Rudxain/dotfiles), for more info
- See also [these naming guidelines](https://github.com/kettanaito/naming-cheatsheet). Some of my repos are not fully compliant, yet.

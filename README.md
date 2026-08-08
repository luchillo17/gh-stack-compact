# gh-stack-skill

Compact agent skill for [`gh stack`](https://github.com/github/gh-stack) — non-interactive rules, **membership**, recipes. Exit codes live in `exits.md` (progressive disclosure).

Not affiliated with GitHub’s official skill (that one is much larger). This one assumes agents can read `gh stack <cmd> --help` and only caches gotchas.

## Install

```bash
npx skills add luchillo17/gh-stack-skill
# or:
npx skills add luchillo17/gh-stack-skill --skill gh-stack
```

Also install the CLI extension (once per machine):

```bash
gh extension install github/gh-stack
```

## Layout

```text
skills/gh-stack/
  SKILL.md    # always-loaded process
  exits.md    # load when non-zero exit and next move unclear
```

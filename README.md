# gh-stack-skill

Compact agent skill **`gh-stack-compact`** for [`gh stack`](https://github.com/github/gh-stack) — non-interactive rules, **membership**, recipes. Exit codes live in `exits.md` (progressive disclosure).

Named to avoid colliding with GitHub’s official **`gh-stack`** skill. Not affiliated. Assumes agents can read `gh stack <cmd> --help` and only caches gotchas.

## Install

```bash
npx skills add luchillo17/gh-stack-skill
# or:
npx skills add luchillo17/gh-stack-skill --skill gh-stack-compact
```

Also install the CLI extension (once per machine):

```bash
gh extension install github/gh-stack
```

## Layout

```text
skills/gh-stack-compact/
  SKILL.md    # always-loaded process
  exits.md    # load when non-zero exit and next move unclear
```

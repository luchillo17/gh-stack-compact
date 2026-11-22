# gh-stack-compact

Compact agent skill **`gh-stack-compact`** for [`gh stack`](https://github.com/github/gh-stack) — non-interactive rules, **membership**, recipes. Exit codes live in `exits.md` (progressive disclosure).

Named to avoid colliding with GitHub’s official **`gh-stack`** skill. Not affiliated. Assumes agents can read `gh stack <cmd> --help` and only caches gotchas.

Origin: [github/gh-stack#377](https://github.com/github/gh-stack/issues/377) (skill verbosity) — [minimal-skill proposal comment](https://github.com/github/gh-stack/issues/377#issuecomment-5147221894).

## Token budget

Rounded counts from `cl100k_base` and `o200k_base`. Re-measure after edits.

| Load                | File       | Tokens |
| ------------------- | ---------- | -----: |
| Always (skill body) | `SKILL.md` |   ~680 |
| On demand           | `exits.md` |   ~430 |
| Worst case (both)   |            | ~1,110 |

## Install

```bash
npx skills add luchillo17/gh-stack-compact
# or:
npx skills add luchillo17/gh-stack-compact --skill gh-stack-compact
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

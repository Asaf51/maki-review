# maki-review

A [[maki](https://github.com/asaf/maki)](https://github.com/tontinton/maki) plugin that adds a `/review` command:
a TUI for reviewing maki's changes, leaving inline comments on diff lines,
and sending them back to a new maki session that fixes them.

<img width="800" height="500" alt="recording2" src="https://github.com/user-attachments/assets/a65e2e8e-54d4-498a-b775-b1444944a798" />

## Features

- **Files** — changed files vs `HEAD` (staged, unstaged, untracked) as a collapsible tree
- **Commits** — recent commits; drill into a commit's files
- **Comments** — every review comment written so far
- **Diff pane** — syntax-highlighted diff with full-row tints; comment a line (`c`),
  select a range first (`v`), delete (`d`)
- **Submit** — `s` sends all comments to a new focused maki session that addresses them
- After each turn, a status flash reminds you when files changed

## Keys

| Key | Action |
| --- | --- |
| `Tab` | cycle left panels |
| `Enter` / `l` | open dir / focus diff / open commit |
| `h` / `Esc` | collapse / back |
| `c` | comment on the current diff line |
| `v` | start range selection |
| `d` | delete comment |
| `s` | submit comments to maki |
| `r` | refresh |
| `q` | quit |

## Install

Copy `review.lua` into your maki plugins directory.

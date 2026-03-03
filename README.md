# uptag

Interactive git tag version bumper for zsh.

Gets the latest semver tag on your main/master branch and bumps it — with a nice TUI or direct flags.

## Install

### Homebrew

```bash
brew install jairaume/tap/uptag
```

### Manual

```bash
git clone https://github.com/jairaume/uptag.git ~/.uptag
ln -s ~/.uptag/bin/uptag /usr/local/bin/uptag
```

## Usage

**Interactive** (default) — arrow keys to pick, Enter to confirm:

```
$ uptag

  ⬆ uptag  — version bumper
  ───────────────────────────
  Current tag: 1.29.0 on main

  ❯ patch   →  1.29.1
    minor   →  1.30.0
    major   →  2.0.0
```

**Direct flags:**

```bash
uptag -p    # patch: 1.29.0 → 1.29.1
uptag -m    # minor: 1.29.0 → 1.30.0
uptag -M    # major: 1.29.0 → 2.0.0
```

Both modes ask for confirmation before creating and pushing the tag.

Press `q` to cancel at any time during interactive selection.

## Requirements

- zsh
- git

## License

MIT

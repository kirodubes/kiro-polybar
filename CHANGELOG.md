# Changelog

## 2026.09.28

### What Changed
- Added `ruff.toml` pinning ruff to the classic rule set. ruff 0.16 widened its implicit rules, so the
  global pre-commit hook started rejecting commits over untouched code (BLE001, PLW1510, I001, ...).

### Technical Details
- Same file as archlinux-tweak-tool: `line-length = 120`, `select = ["E4", "E7", "E9", "F"]`, `E402`
  ignored for `gi.require_version()`. `ruff check .` passes with no code changes.

### Files Modified
- `ruff.toml` (new)

## 2026.05.25

### What Changed
- De-brand (user-visible): the `[module/jgmenu]` polybar module ran
  `echo "ArcoLinux"`, displaying that text in the bar. Changed to `echo "Kiro"`.
  Part of the ecosystem-wide arcolinux de-brand sweep.

### Files Modified
- `etc/skel/.config/polybar/config.ini`

## 2026.05.21

### What Changed
- Initial markdown scaffold added per the ecosystem MD-scaffold rule ([HQ/CLAUDE.md](/home/erik/Insync/Kiro/Kiro-HQ/CLAUDE.md#required-markdown-scaffold-every-repo)).
- Stubs created for `CHANGELOG.md`, `CLAUDE.md`, `IDEAS.md`, `TODO.md` (whichever were missing).
- README rewritten with real install/usage content (replaced earlier one-line stub) where applicable.

### Files Modified
- CHANGELOG.md (created)
- CLAUDE.md (created where missing)
- IDEAS.md (created where missing)
- TODO.md (created where missing)
- README.md (rewritten where it was a stub)

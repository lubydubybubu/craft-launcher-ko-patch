# craft-launcher-ko-patch

Korean (한국어) interface patch for **[ArtCraft Launcher](https://github.com/storytold/craft-launcher)** (installer/updater for the Craft apps), upstream tag `v0.3.2`.
This repository contains **only the patch**, not ArtCraft Launcher's source code. See `BASE.txt` for the exact upstream commit.

## Apply
```bash
git clone --branch v0.3.2 https://github.com/storytold/craft-launcher.git && cd craft-launcher
git apply ../craft-launcher-ko-patch/patches/craft-launcher-v0.3.2-ko.patch
```
Then build as upstream documents. Windows build without MSVC: [artcraft-ko-toolkit](https://github.com/lubydubybubu/artcraft-ko-toolkit).

## What it changes
Korean catalog ported from storytold/craft-launcher PR #285 (back2zion) plus Korean/system font support; keys completed against the most complete catalog.
Changed files: `CHANGED-FILES.txt`.

## Verified
6 Korean + 28 i18n + 5 font tests on Linux; on Windows the Korean UI integration test passes and renders grid/settings snapshots in Korean without tofu.

## Known limits
Only the Korean parts of PR #285 were taken.

Translations are AI-assisted (Claude Opus 5.5) and not reviewed by a professional translator.
Licence: MIT OR Apache-2.0, same as ArtCraft Launcher; upstream contributions credited above.

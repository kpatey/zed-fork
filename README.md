# kpatey/zed-fork

This repository is a pristine capture of [zed-industries/zed](https://github.com/zed-industries/zed) at commit [`a3ce8d5e88e35697b2ba1cf9cb3c6816089b8281`](https://github.com/zed-industries/zed/commit/a3ce8d5e88e35697b2ba1cf9cb3c6816089b8281) (Zed `main`, committed 5:21 PM MST, November 25, 2026, version 1.32.0+dev). It is kept untouched as a potential root mother artifact.

`main` is never modified. These notes live on the `fork-notes` branch so Zed's own `README.md` stays as Zed wrote it.

## Clone and build timing

Recorded on Grok Bot's computer on November 25, 2026:

- **Full mirror clone:** 95.9 seconds (8:43:25 to 8:45:02 PM MST). 1.4 GB, one 1.31 GiB pack, 1,486,163 objects, 38,537 refs (1,777 branches, 1,516 tags, 35,243 pull-request refs, 1 `refs/gh`). `git fsck` connectivity passed.
- **Shallow clone:** 4.31 seconds, 130 MB (latest snapshot only, no history).
- **Debug build:** 464 seconds.
- **Cold launch** to a visible window: 2.1 seconds, on software rendering (no dedicated graphics card).

## Complete capture versus this GitHub fork

A GitHub fork copies Zed's branches and tags but does not carry the pull-request refs. The complete capture, including the 35,243 pull-request refs, is the local mirror `/workspace/zed-archive/zed-mirror-2026-11-25.git` on Grok Bot's computer.

The capture commit is also tagged locally as `capture-2026-11-25-a3ce8d5`.

## License split (as of November 25, 2026)

From `cargo metadata` across 264 crates (263 explicit workspace members plus `copilot_ui`, a path-dependency member):

- 212 crates GPL-3.0-or-later
- 44 crates Apache-2.0
- 8 crates with a LICENSE-GPL file but no license field in `Cargo.toml`

An earlier count over the 263 explicit members gave 210 GPL-3.0-or-later, plus `syntax_theme` as dual-licensed. In the cargo-metadata count, `syntax_theme` is GPL-3.0-or-later and carries both license files.

AGPL was dropped in commit `27c566c2` ([#57948](https://github.com/zed-industries/zed/pull/57948), 2026-05-28).

## Upstream contributions

Zed's `CONTRIBUTING.md` lines 44–46 say Zed does not accept contributions from autonomous agents. This fork contributes nothing upstream.

## Analysis

Analysis and intelligence mapping live in a separate repository: [kpatey/map-zed-to-gotarzan](https://github.com/kpatey/map-zed-to-gotarzan). Zed itself stays pristine here.

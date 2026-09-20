# Pinchy releases

Download **Pinchy**, the helpful blue lobster for your desktop, from the [latest release](../../releases/latest):

| Your computer | File |
|---|---|
| Linux | `BlueLobster-<version>.AppImage` (make it executable, then start it) |
| Windows | `BlueLobster-Setup-<version>.exe` (installer) or `BlueLobster-Portable-<version>.exe` (no install) |
| macOS (Apple silicon) | `BlueLobster-<version>-mac-arm64.zip` |
| macOS (Intel) | `BlueLobster-<version>-mac-x64.zip` |

You only need to do this once. From version 1.1.0 on, Pinchy updates himself: he tells you when a new version is
out, you click **Update now**, and he comes back a few seconds later (Settings → Safety & data → Updates).

**How updates are kept safe.** Every release carries `latest.json` (the list of files with their sizes and SHA-256
checksums) and `latest.json.sig`, a signature made with a key that never leaves the maintainer's computer. Pinchy
ignores any list that is not signed with that key, never installs an older version than the one he is, and deletes
any download that does not match the signed checksum. The builds are not code-signed, so Windows SmartScreen and
macOS Gatekeeper will ask once on the first manual install.

This repository holds finished builds only. The source code is not public.

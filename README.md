# Reglaize updates

The Reglaize desktop app checks this repository's releases for updates.
Each platform and channel has one fixed release (`windows-x64-estable`, `macos-arm64-estable`) whose files are
replaced on every version: a signed `manifest.json`, its `manifest.json.sig` (Ed25519) and the versioned zip.

Files here are published by `build/publica.py` in the Reglaize repository. Do not edit them by hand: the app
refuses any manifest that is not signed with the key it carries.

# GhostQuill Releases

Public release feed and binaries for **GhostQuill** — a macOS menu-bar app for
push-to-talk voice typing, powered by on-device [whisper.cpp](https://github.com/ggml-org/whisper.cpp)
transcription.

## What lives here

- [`appcast.xml`](appcast.xml) — the [Sparkle](https://sparkle-project.org/) update
  feed the app checks. Feed URL:
  `https://raw.githubusercontent.com/szaycev/ghostquill-releases/main/appcast.xml`
- [Releases](../../releases) — downloadable builds, one tag per version
  (`v{version}`): a `.dmg` for first installs and a `.zip` the in-app updater
  consumes.
- [`notes/`](notes) — the release-note fragments embedded in the feed.

## Update integrity

Every update archive is signed with an EdDSA (Ed25519) key; the app only
installs updates whose signature matches the public key it ships with:

```
7Jya4jR8KR1v5XDAcIPGAF8PoJIz0BtafQeF3tB+cJw=
```

Entries in this repository are produced by GhostQuill's release pipeline, not
edited by hand.

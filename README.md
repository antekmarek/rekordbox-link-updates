# Rekordbox Link updates

Audio-reactive club visuals for Windows by Antoni Marek ([antekmarek.com](https://antekmarek.com)).

This repository is only the **update channel**: every release holds a signed `manifest.json` and the files it
names. The installed app reads
`https://github.com/antekmarek/rekordbox-link-updates/releases/latest/download/manifest.json` when it starts.

- **Small updates** (`pack-<version>.zip`, the app's own code and pictures) download in the background. They are
  used after the app restarts.
- **Full updates** (`RekordboxLink-Setup-<version>.exe`) install with one click from the app's menu.

Every manifest is signed with Ed25519. The app refuses a manifest that its built-in key does not verify, and any
file whose SHA-256 differs from the signed manifest. To install for the first time, download the newest
`RekordboxLink-Setup-*.exe` from [Releases](https://github.com/antekmarek/rekordbox-link-updates/releases).

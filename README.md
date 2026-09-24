# Phone Booth — releases

Installers and updates for Phone Booth, the phone booth art installation. The source is
private; this repo holds only the published releases.

## Install on a new Mac

Open Terminal and paste this line once:

```
curl -fsSL https://github.com/emmettjez/phonebooth-releases/releases/latest/download/install.sh | bash
```

It downloads the latest release, checks it, installs it into `~/PhoneBooth/app/`,
asks which language model to download, builds **Phone Booth.app**, pins it to the Dock
and turns on Start at login. The first run downloads several GB of models.

Needs macOS 13 or later and the Xcode Command Line Tools (`xcode-select --install`).

## Updating

In the control panel: **SETTINGS › Maintenance › Check for Updates**, then **Update…**.
The booth saves a snapshot first, installs the new version beside the running one,
tests it, and restarts when no call is up. **Go Back…** returns to the previous
version. Nothing checks or updates on its own.

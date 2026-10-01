# Phone Booth — releases

Installers and updates for Phone Booth, the phone booth art installation. The source is
private; this repo holds only the published releases.

## Install on a Mac

Open Terminal and paste this line once:

```
curl -fsSL https://github.com/emmettjez/phonebooth-releases/releases/latest/download/install.sh | bash
```

It downloads the latest release, checks it, installs it into `~/PhoneBooth/app/`,
asks which language model to download, builds **Phone Booth.app**, pins it to the Dock
and turns on Start at login. The first run downloads several GB of models.

Needs macOS 13 or later and the Xcode Command Line Tools (`xcode-select --install`).

## Install on Linux (Ubuntu 24.04)

Open a terminal and paste this line once:

```
wget -qO- https://github.com/emmettjez/phonebooth-releases/releases/latest/download/install.sh | bash
```

It asks for the computer's password once (for the sound library, the phone's ethernet
port and, with an NVIDIA card, CUDA), asks for a Console Passcode, and starts the booth.
No screen is needed afterwards: the booth starts at power-on with nobody logged in, and
you run it from the console on any device on the network. With an NVIDIA graphics card,
Talkback and Transcripts run on the card.

## Install links

An admin can send an install link from **SETTINGS › STORAGE › Send Install Link…**. It
opens a page with the same line, ready to paste, that also signs the new computer in to
the Cloud. Installing never needs an account; signing in only puts a computer on the
Cloud.

## Updating

In the control panel: **SETTINGS › Maintenance › Check for Updates**, then **Update…**.
The booth saves a snapshot first, installs the new version beside the running one,
tests it, and restarts when no call is up. **Go Back…** returns to the previous
version. Nothing checks or updates on its own.

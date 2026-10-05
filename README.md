# phonema Spot downloads

**phonema Spot v0.1** is a preview release for macOS 13 or later, available as a universal app for Apple silicon and Intel.

## Download

- [Download phonema Spot v0.1 from Cloudflare](https://spot.phonema.audio/downloads/phonema-spot-0.1-universal.dmg)
- [Download its SHA-256 checksum](https://spot.phonema.audio/downloads/phonema-spot-0.1-universal.dmg.sha256)
- [GitHub mirror for the first migration release](https://github.com/emilianomArg/Holocron-Downloads/releases/tag/v0.1)

The DMG is encrypted with AES-256. Open it using the same password previously supplied for your installer; contact the distributor if you need it.

This preview has an ad hoc signature. Developer ID signing and Apple notarization are still pending, so macOS may display an unidentified-developer or verification warning.

Downloading, installing, or using phonema Spot is subject to the [End User License Agreement](EULA.md), also included in the installer.

## Install and migrate

Quit the previous app, open the DMG, and drag `phonema Spot.app` into Applications. On first launch, the app migrates your existing sound index and recognized preferences. Your audio libraries remain in their existing locations.

Once installed, phonema Spot checks for future updates at [spot.phonema.audio](https://spot.phonema.audio). Support reports are submitted only when you choose **Send to Support** in an error dialog.

## Why this repository keeps its previous name

Existing EM Holocron installations still read this repository's update feed and require its original GitHub release path. The repository name remains `Holocron-Downloads` temporarily so those users can install phonema Spot.

The old app may show an update announcement numbered **0.10**. That number triggers its existing version comparison; the app downloaded and installed is **phonema Spot v0.1**.

The v0.1 installer is mirrored here for this transition. Future phonema Spot releases use Cloudflare.

# EM Holocron downloads

Public update metadata and release downloads for EM Holocron. The application
source remains in a separate private repository.

Downloading, installing or using EM Holocron is subject to the
[End User License Agreement](EULA.md). Version 0.8 and later also presents the
agreement for acceptance on first launch. Release DMGs are encrypted for the
studio and the password is distributed separately.

## Publishing a version

1. Store the studio DMG password in the `EM-Holocron-DMG` macOS Keychain item.
2. Build `EM-Holocron-<version>-universal.dmg` and its `.sha256` file in the
   private source repository with `Scripts/build_release_dmg.sh`.
3. Create tag and GitHub Release `v<version>` here and attach both files.
4. Update `latest.json`: `latest_version`, `release_url` and `notes`.
5. Commit and push to `main`.
6. Verify `https://raw.githubusercontent.com/emilianomArg/Holocron-Downloads/main/latest.json`.

GitHub Pages is not required. The app reads the public repository's raw JSON
directly. The value of `release_url` must remain an HTTPS URL on `github.com`;
the app rejects other hosts.

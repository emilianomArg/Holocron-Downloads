# EM Holocron downloads

Public update metadata and release downloads for EM Holocron. The application
source remains in a separate private repository.

## Publishing a version

1. Build `EM-Holocron-<version>-universal.dmg` and its `.sha256` file in the
   private source repository with `Scripts/build_release_dmg.sh`.
2. Create tag and GitHub Release `v<version>` here and attach both files.
3. Update `latest.json`: `latest_version`, `release_url` and `notes`.
4. Commit and push to `main`.
5. Verify `https://raw.githubusercontent.com/emilianomArg/Holocron-Downloads/main/latest.json`.

GitHub Pages is not required. The app reads the public repository's raw JSON
directly. The value of `release_url` must remain an HTTPS URL on `github.com`;
the app rejects other hosts.

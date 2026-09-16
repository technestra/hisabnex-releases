# Hisabnex releases

Public home for the Hisabnex Android builds. The app source stays in a private repository; only the
installable file and the version note live here.

- `latest.json` — the file the app reads in Settings > App Update. It names the current version and where
  the APK is.
- **Releases** — every build is uploaded as a release asset named `hisabnex-latest.apk`, so the download
  link never changes.

## Publishing a build

1. Create a new release with a tag like `v1.3`.
2. Upload the signed APK as `hisabnex-latest.apk` (a copy named `hisabnex-1.3.apk` is optional).
3. Update `versionCode`, `versionName` and `notes` in `latest.json` on the `main` branch.

Every build is signed with the same key, so a phone refuses anything not built by us.

Hisabnex is a product of [Wheatron Technologies](https://wheatrontechnologies.com/).

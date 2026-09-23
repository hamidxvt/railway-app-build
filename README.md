# railway-app-build

Release distribution repo for the Bookmark Field Force Manager mobile app.

This repo holds no source code. Its GitHub Actions workflow checks out
the private source repo, builds and signs the release APK, and publishes
it here as a GitHub Release — so the app's in-app update check can
download the APK without needing any authentication (the source repo
stays private; this repo is public and holds only build outputs).

To build and publish a new release, run the **Build & Release APK**
workflow from the Actions tab (or `gh workflow run build-apk.yml`).

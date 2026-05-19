# BadHabit releases

Public release artifacts for the [BadHabit](https://github.com/bekov001/badhabit) app (source is private).

- `latest.json` — current version manifest (consumed by the app for in-app update checks)
- `downloads/` — APK files

Update flow:
1. Build new APK
2. Copy into `downloads/`
3. Bump `latest.json` (`versionCode`, `versionName`, `url`, `releasedAt`, `notes`)
4. Commit + push
5. App detects new version on next launch and shows update banner

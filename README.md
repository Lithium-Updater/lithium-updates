# Lithium Launcher Updates

Hosts update manifests and zips for the Lithium Launcher auto-update engine.

## How to release a new version

1. Build the new version zip (e.g. `Lithium-Launcher-v1.2.3.zip`)
2. Place it in this repo
3. Edit `update.json`:
   - Bump `"version"` to the new version
   - Change `"url"` to point to the new zip
   - Update `"changelog"` and `"changelogFull"`
4. Commit and push

## URL format

The launcher reads from:
```
https://lithiumlauncher.github.io/updates/update.json
```

Set this URL in the launcher: Settings → Launch Options → Update check URL

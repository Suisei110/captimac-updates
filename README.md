# CaptiMac Updates

Sparkle 2 appcast feed for CaptiMac — macOS UGC caption generator.

## Live Feed

```
https://suisei110.github.io/captimac-updates/appcast.xml
```

## Release Assets

DMG files hosted on the public [captimac-releases](https://github.com/Suisei110/captimac-releases) repo.

## How It Works

1. New DMG uploaded to `captimac-releases` via GitHub Releases
2. `appcast.xml` in this repo updated with new `<enclosure>` URL + Sparkle Ed25519 signature
3. GitHub Pages serves the updated feed instantly
4. CaptiMac's Sparkle updater fetches the feed and downloads updates

## Repository

- **Static hosting** via GitHub Pages (branch `main`, root)
- No build step required

---

© 2026 Randy Rakhman

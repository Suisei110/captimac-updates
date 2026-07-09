# CaptiMac Updates Repository

This repository hosts the Sparkle appcast and release metadata for direct-distribution builds of CaptiMac.

## Live appcast

- URL: `https://suisei110.github.io/captimac-updates/appcast.xml`
- Used by `SUFeedURL` in CaptiMac's Info.plist.

## How updates are published

1. In the main CaptiMac repo, run:
   ```bash
   ./scripts/generate_appcast.sh \
     --version 2.3.1 \
     --dmg-url "https://github.com/Suisei110/captimac/releases/download/v2.3.1/CaptiMac-2.3.1.dmg" \
     --private-key ~/Documents/captimac_keys/sparkle_private.pem
   ```
2. The script outputs a new `appcast.xml`.
3. Copy that file to this repository and push to `main`.
4. GitHub Pages will automatically serve the updated appcast.

## Repository settings

- Source: GitHub Pages → Deploy from a branch → `main` → `/ (root)`.
- No build step is needed; this repo only serves static XML.

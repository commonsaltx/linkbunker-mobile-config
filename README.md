# linkbunker mobile config (public mirror)

`mobile-config.json` is the fallback copy of `GET https://api.linkbunker.com/v1/mobile/config`,
read by the linkbunker mobile apps when the API cannot be reached within four seconds.
It holds no secrets: the minimum native app version per platform, the store links, the release
stage and feature overrides, and when it was written.

The API is the source of truth. This file is regenerated from the main repository with
`node scripts/mobile-config-snapshot.mjs <api base>` whenever the minimum version changes.

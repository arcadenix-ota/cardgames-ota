# cardgames-ota

OTA (hot update) content for the card games client (Cocos Creator 3.8).

- `main` holds only small pointer files under `latest/` (e.g. `latest/android.json`) telling clients which immutable ref to load.
- Build content lives on separate branches/tags and is served via jsDelivr at an exact tag or commit sha:
  `https://cdn.jsdelivr.net/gh/arcadenix-ota/cardgames-ota@<tag-or-sha>/...`
- Pointer files are read from `raw.githubusercontent.com` with jsDelivr `@main` as fallback.

Release order: push content branch + tag first, then update the pointer on `main`.

# FortByte-Patched-Builds

> **This is not a Fortnite build archive.** It's the download host for the
> **FortByte** Android launcher — the redirect-patched Fortnite APKs it installs,
> plus the catalog that lists them. If you're here looking for clean/unmodified
> builds, this isn't that.

Every APK here is a vanilla Fortnite Android build with the **Moonwave** redirect
baked in, so the game talks to a self-hosted OGFN backend instead of Epic. You
don't grab these by hand — the FortByte app reads [`builds.json`](builds.json),
shows you the versions, and pulls the one you pick straight from this repo's
**[Releases](../../releases)**.

## What's in here
- **`builds.json`** — the catalog the app fetches: `id`, season/chapter, `sizeBytes`, `sha256`, and the release `downloadUrl` for each build.
- **Releases** — one release per version (tag = build id, e.g. `7.40`), with the APK attached as `<id>.apk`. APKs live in releases because they're >100 MB — GitHub caps repo files at 100 MB but allows up to 2 GB per release asset.

## How you actually use it
1. Install the **FortByte app** (soon).
2. In Settings, point it at your backend (IP\:port).
3. Pick a version → **Download** → **Install** → launch. Done.

### About teh FortByte app
Soon / later

> These builds are Android-debug-signed, so they can't install *over* a store
> copy of Fortnite (signature mismatch) — uninstall that first. The FortByte app
> detects this and walks you through it. Each build is also labelled
> `Fortnite <version>` on the home screen so you can tell them apart.

*For testing / private-server use only.*

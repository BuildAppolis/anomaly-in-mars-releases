# NEON DRIFT releases

Builds of NEON DRIFT, a native arena shooter for Windows. This repository holds
binaries only; the source lives elsewhere.

Each release carries two assets:

- `NeonDrift-<version>.exe` - the game, one file, no installer. Put it anywhere
  and run it; settings and scores are kept beside it.
- `latest.json` - the manifest the game reads. It names the newest build, its
  SHA-256 and where to fetch it.

The game checks this repository's newest release on its title screen. If it
finds a newer version it offers to download it beside the running one, verifies
it against the checksum in the manifest, and restarts into it. To install by
hand, download the `.exe` from the latest release.

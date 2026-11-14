# Changelog

All notable changes to Krelzox OS are documented here. Versions follow
[Semantic Versioning](https://semver.org/); `-alpha` releases are previews.

## [0.1.0-alpha] — 2026-11-14

First public preview. Three Android TV apps for the Raspberry Pi 5
(LineageOS 24.0 `rpi5_tv`, Android TV 17).

### Krelzox Launcher (`dev.krelzox.launcher`)
- Home screen with a dynamic hero (*Continue*, recents, favorites,
  suggestions), favorites with live reordering, and Library and Media tabs.
- Full D-pad navigation with hierarchical Back; touch and click support.
- Performance monitor: top-bar panel (CPU, RAM, temperature, storage), live
  charts and a System & performance center. Real values only.
- Four themes (Ion, Aurora, Amber, Jade) and the Krelzox screensaver.
- Safe mode after repeated crashes; the stock launcher is never disabled.
- One normal permission; no root, telemetry, ads or network server.

### Krelzox Store (`dev.krelzox.store`)
- Catalog from F-Droid-format repositories (f-droid.org by default), with
  search, categories, app pages, favorites and history.
- Real installs, updates and uninstalls through Android's installer, after
  verifying the signed index (pinned key, no rollback) and each APK's size,
  SHA-256, package, version and signing certificate.

### Krelzox Remote (`dev.krelzox.remote`)
- Watch and control the TV from a browser on the local network: Touch,
  Trackpad and Remote modes, media and volume keys, typing, opening apps.
- Off by default and LAN-only; one-time PIN pairing; control approved on the
  TV with *Deny* selected by default.

### Known limitations
- Krelzox Remote's traffic is not encrypted (use it on a trusted network) and
  its picture is JPEG, not compressed video. It has been tested on the Pi with a
  scripted client, not yet from a phone browser.
- Krelzox Store has no ratings, reviews or background update checks.
- Only tested on the reference Raspberry Pi 5 build.

[0.1.0-alpha]: https://github.com/Nach0t/Krelzox-OS/releases/tag/v0.1.0-alpha

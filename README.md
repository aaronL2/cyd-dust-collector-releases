# CYD Dust Collector — firmware

Built images only. **Source is in a separate private repository.**

This repo exists so collectors and stations can fetch their own updates over
HTTP without a credential on the device, which is why it is public. It holds
no source, no credentials, and no per-unit secrets — SoftAP passwords are
generated on each device and stored in its NVS, never compiled in.

| File | Role |
|------|------|
| `station.bin`   | station firmware |
| `collector.bin` | collector firmware |
| `manifest.json` | current build stamps, sizes, MD5s, URLs |

Stamps are `YYYYMM.DD.HH.MM` of the build, shown on-device as `FW: …`.

Current: **202610.06.15.50**

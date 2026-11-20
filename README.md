# Loco Mart POS — Releases

Downloads for the **Loco Mart POS** apps. The source code is private; this
repository only hosts the compiled apps and their update feeds.

## Apps

| App | What it is | Download |
|---|---|---|
| **Loco Mart POS** | The point-of-sale app for Android phones | [Releases](../../releases) — tags `pos-v…` |
| **Loco Mart SMS** | The SMS gateway phone: sends texts for Loco Mart POS and forwards MTN MoMo payment alerts | [Latest](../../releases) — tags `sms-v…` |

## Installing

1. Open the release you want and download the `.apk` file on the phone.
2. Open it. Android asks once to allow installing apps from your browser or
   file manager; allow it.
3. Later versions install as updates, keeping the app's settings. Loco Mart
   SMS finds them itself: **Settings → Check for updates**.

## Update feeds

Each app checks its own feed, so the apps never pick up each other's updates:

- `sms-gateway/latest.json` — Loco Mart SMS
- `pos/latest.json` — Loco Mart POS

```json
{ "version": "1.6.0", "versionCode": 13, "apkUrl": "https://github.com/…/Loco-Mart-SMS_1.6.0.apk",
  "notes": "What changed", "pub_date": "2026-11-20T15:00:00Z", "sha256": "…" }
```

Releases and feeds are published with `release/publish-release.ps1` in the
source repository.

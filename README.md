# Mavin Ops — release channel

Public download + auto-update channel for the **Mavin Ops** Android app (a Star
Citizen mining / refinery / payout tracker). The app's **source code is private**;
this repo holds only the built APKs and a small `version.json` that the app reads
to offer in-app updates.

## Install / download

Grab the latest APK from the [**Releases**](../../releases/latest) page and open
it on your Android device. You'll get Android's normal "install unknown apps"
confirmation (that's expected for a sideloaded app).

## Auto-update

Once installed, the app checks this channel on launch and offers a one-tap update
when a newer build is posted here — no Play Store needed. `version.json` always
points at the current release:

```json
{ "version": "1.35.0", "apkUrl": ".../releases/download/v1.35.0/mavin-ops-1.35.0.apk", "notes": "…" }
```

The web app (https://mavin-ops.web.app) updates itself on reload and isn't
affected by this channel.

# TempBridge Web

Static Web Bluetooth client for the TempBridge BLE bridge. This repository
contains no sensor firmware, bridge firmware, measurements, or sensor MAC.

## Publish with GitHub Pages

1. Push these files to the `main` branch of a GitHub repository.
2. Open **Settings > Pages** in that repository.
3. Select **Deploy from a branch**, branch `main`, folder `/(root)`.
4. Open the HTTPS address displayed by GitHub in Chrome for Android.

Tap **Connect**, select `TempBridge`, then use **Sync history** and **Export
CSV**. The page talks directly to the bridge over BLE; GitHub only hosts the
static HTML and does not receive the sensor measurements.

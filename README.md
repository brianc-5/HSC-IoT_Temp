# TempBridge Web

Static Web Bluetooth client for the TempBridge BLE bridge. This repository
contains no sensor firmware, bridge firmware, measurements, or sensor MAC.

## Publish with GitHub Pages

1. Push these files to the `main` branch of a GitHub repository.
2. Open **Settings > Pages** in that repository.
3. Select **Deploy from a branch**, branch `main`, folder `/(root)`.
4. Open the HTTPS address displayed by GitHub in Chrome for Android.

Tap **Connect**, select `TempBridge`, then use **Sync history** and **Export
CSV**. The page reports the automatically detected bare/HAT and USB/external
configuration, displays the sensor's reported cadence, and enables only the
measurements and power analysis supported by that configuration. The bridge
and page accept arbitrary sensor cadences without source changes. History opens
in a one-hour view with 30-minute, 1-hour, 2-hour, 6-hour, 12-hour, and full
retention choices; use the scrubber, Older/Newer buttons, or drag the chart
horizontally to move through time.

The page talks directly to the bridge over BLE; GitHub only hosts the static
HTML and does not receive the sensor measurements.

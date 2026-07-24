# TempBridge Web

Static Web Bluetooth client for the TempBridge BLE bridge. This repository
contains no sensor firmware, bridge firmware, measurements, or sensor MAC.

## Publish with GitHub Pages

1. Push these files to the `main` branch of a GitHub repository. Deploy
   `chart.umd.js` next to `index.html`: the page loads it from the same
   origin, which works with no internet connection and contacts no third
   party. If it is missing, the page falls back to a subresource-integrity
   pinned copy on jsDelivr, and to the table and CSV export if that also fails.
2. Open **Settings > Pages** in that repository.
3. Select **Deploy from a branch**, branch `main`, folder `/(root)`.
4. Open the HTTPS address displayed by GitHub in Chrome for Android.

Tap **Connect**, select `TempBridge`, then use **Sync history** and **Export
CSV**. The page reports the automatically detected bare/HAT and USB/external
configuration, displays the sensor's reported cadence, and enables only the
measurements and power analysis supported by that configuration. The bridge
and page accept arbitrary sensor cadences without source changes.

The page talks directly to the bridge over BLE; GitHub only hosts the static
HTML and does not receive the sensor measurements.

# WitAqua WayDroid OTA

OTA channels for WitAqua WayDroid images, in the format waydroid reads.

```sh
sudo waydroid init -f \
    -c https://witaqua-waydroid.github.io/ota/16.2/system \
    -v https://witaqua-waydroid.github.io/ota/16.2/vendor \
    -s VANILLA    # or GAPPS
```

Requires waydroid 1.6.3 or newer with libgbinder 1.1.45 or newer on the host
(Android 16 needs the aidl6 service manager protocol).

| Channel | Path |
|---|---|
| system | `16.2/system/lineage/<device>/<VANILLA\|GAPPS>.json` |
| vendor | `16.2/vendor/<device>/MAINLINE.json` |

The JSON files are updated by the build pipeline
([WitAqua-WayDroid/build-config](https://github.com/WitAqua-WayDroid/build-config)).

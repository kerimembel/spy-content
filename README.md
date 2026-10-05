# SPY game catalog

The SPY app reads [catalog.v1.json](catalog.v1.json) over HTTPS when it opens and when it returns to the foreground. Changes may take a few minutes to appear because GitHub caches raw files and the app refreshes at most every five minutes. The last valid version is cached on device; the app also has a bundled fallback.

[Public SPY page](https://kerimembel.github.io/spy-content/spy/) · [Privacy](https://kerimembel.github.io/spy-content/spy/privacy.html) · [Support](https://kerimembel.github.io/spy-content/spy/support.html)

To update the game without an app release, edit `catalog.v1.json` in GitHub, increase `revision`, and commit. Each category needs English and Turkish `name`, `sub`, and 8–80 word pairs per language. Pair difficulty is `easy`, `medium`, or `hard`. Add a pack with `tier` set to `owned`, `premium`, or `adult` and list its category IDs. A pack category can belong to only one pack. Adult pairs must belong to an adult pack. To remove existing content, use `removePacks` and/or `removeCategories` arrays. Invalid updates are ignored by the app.

`owned` packs are free; `premium` and `adult` packs use the existing SPY+ entitlement. This file changes words and pack access, but cannot add a new in-app purchase product or change subscription prices.

All data in this repository is public. Do not add credentials or private information.

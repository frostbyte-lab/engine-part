# Engine Part Catalog

Master catalog data for the Engine Part Android application. The Android app expects `catalog.json` to follow the schema in the application project and uses explicit numeric IDs for all relationships.

## Update catalog

Edit `catalog.json`, validate it as JSON, commit, and push to `main`. The Android application synchronizes the catalog when it starts and periodically when network access is available.

For public direct access, use:

`https://raw.githubusercontent.com/frostbyte-lab/engine-part/main/catalog.json`

If this repository remains private, serve the file through an authenticated Cloudflare Worker or another protected proxy; raw GitHub access from an unauthenticated Android app will not be reliable.

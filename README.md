# Engine Part Catalog

Master catalog data for the Engine Part Android application. The Android app expects `catalog.json` to follow the schema in the application project and uses explicit numeric IDs for all relationships.

## Current coverage

The current public feed contains sourced Mitsubishi model metadata for 2015 and the latest official lineup reference, including Mitsubishi Motors and Mitsubishi Fuso. It intentionally does not invent or bulk-copy OEM part numbers. Exact part fitment depends on market, trim, engine code, VIN/chassis, and model year.

To complete the part-number layer, add a licensed OEM/dealer export and include `spareparts`, `partNumbers`, `compatibilities`, and `images` records with source fields and verification status. Records without a reliable source must remain `UNVERIFIED`.

## Update catalog

Edit `catalog.json`, validate it as JSON, commit, and push to `main`. The Android application synchronizes the catalog when it starts and periodically when network access is available.

For public direct access, use:

`https://raw.githubusercontent.com/frostbyte-lab/engine-part/main/catalog.json`

## Sources

- Mitsubishi Motors parts storefront: https://parts.mitsubishicars.com/
- Mitsubishi Motors 2015 Outlander press kit: https://media.mitsubishicars.com/en-US/releases/release-a8a2ecf83b4f4524b65fa6c9f39fe478-2015-outlander-press-kit
- Mitsubishi Motors current models: https://www.mitsubishicars.com/cars-and-suvs
- Mitsubishi Fuso Genuine Parts: https://www.mitsubishi-fuso.com/en/parts-services/parts-accessories/genuine-parts/

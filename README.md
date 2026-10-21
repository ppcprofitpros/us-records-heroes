# us-records-heroes (staging)

County hero images for usrecords.org, staged for one mechanical ingest by Lovable. Delete this repo's contents after ingest.

- `done/` finished heroes (1600x900, navy flat overlay #0b2b4a at 65%, slight desaturate, WebP + AVIF twin). Names are `{county-slug}-{state}.webp|avif`.
- `needs-variation/` raw best-available photos. Lovable's AI must vary each, then apply the recipe (16:9 crop to 1600x900, saturation 0.95, contrast 1.03, flat #0b2b4a at 65%, WebP <= ~40 KB, AVIF <= ~18 KB).
- `manifest.json` one row per county: state, county, slug, base, folder (done, needs-variation, none), file, license, credit, source_page, notes. `none` means no usable image; the page uses the fallback chain.
- `CREDITS.md` credit lines required for CC BY and CC BY-SA images in `done/`. Public domain and CC0 need no credit.

Counts: 475 counties (KS 105, VA 133, TN 95, OR 36, WA 39, FL 67): 398 done, 68 needs-variation, 9 none.

# TARS cases

Keep every demonstration asset in this directory. Do not place case videos or posters elsewhere in the repository.

## Current scaffold

The live page preserves all original Top Cases, More Cases, comparison, carousel, waterfall-grid, and “Show More Cases” positions. All 87 former media positions now render as placeholders, so no legacy video is loaded or needed.

Recommended TARS groups are initial viewpoint plus camera-motion control, portrait first-person-to-third-person, portrait third-person-to-first-person, and animal third-person-to-first-person. Robotic-arm scenes are reserved for the featured Top Cases only and are intentionally not duplicated in More Cases.

When final files arrive, keep them in case/ and provide the desired category, display order, and caption; the placeholders can then be bound without changing the page structure.

Archived 12-slot draft:

- `trajectory-01` through `trajectory-03`
- `viewpoint-01` through `viewpoint-03`
- `reverse-angle-01` through `reverse-angle-03`
- `perspective-01` through `perspective-03`

For each slot, provide:

```text
case/<slot>.mp4
case/<slot>.webp   # optional poster image
```

Once assets are available, replace the matching placeholder in `index.html` with:

```html
<video playsinline controls loop preload="none"
  data-poster="case/<slot>.webp"
  data-src="case/<slot>.mp4"></video>
```

Each video should contain its own reference/result or comparison labels when they are needed for interpretation. Please also provide the desired category, display order, and caption for every case.

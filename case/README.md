# TARS cases

Keep every demonstration asset in this directory. Do not place case videos or posters elsewhere in the repository.

## Current scaffold

The live page preserves all original Top Cases, More Cases, comparison, carousel, waterfall-grid, and “Show More Cases” positions. All 87 former media positions now render as placeholders, so no legacy video is loaded or needed.

Recommended TARS groups are camera trajectory control, large-motion re-shooting and novel-region synthesis, text-guided viewpoint control, reverse-angle re-shooting, and first-/third-person perspective switching. Driving and embodied-agent examples are also strong application cases from the paper.

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

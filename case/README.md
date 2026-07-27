# TARS cases

Keep every demonstration asset in this directory. Do not place case videos or posters elsewhere in the repository.

Current featured slots:

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

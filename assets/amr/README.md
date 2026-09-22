# AMR Built From Scratch — image assets

Drop the real photos for the "AMR Built From Scratch" project into this folder using the
filenames below. The site will reference these paths directly (`assets/amr/<filename>`).

No images currently exist here — none have been invented or generated. This README is a
placeholder until the real files are added.

## Recommended filenames

| Filename | Purpose |
|---|---|
| `amr_full.jpg` | Completed robot — primary hero image for the project card |
| `amr_build_01.jpg` | Mechanical / electrical build (integration in progress) |
| `amr_build_02.jpg` | Additional build / integration image |
| `amr_lidar.jpg` | Sensor / dual-LiDAR setup (if available) |

## Notes for Phase 3 implementation

- Only `amr_full.jpg` is treated as required; the other three are optional.
- Each `<img>` should fail gracefully (e.g. an `onerror` fallback that hides the broken image
  and/or swaps in a neutral placeholder block) so a missing optional file never renders as a
  broken-image icon.
- Do not add any image here that wasn't manually placed — this directory is asset storage
  only, not something to be populated automatically.

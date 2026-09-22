# Humanoid technical evidence

Public-facing visual evidence supporting the Humanoid case study's Kinematics &
Real-Time Mapping section ("Kinematic Mapping & Operating-Range Analysis"), wired
into `index.html` in Phase 5.5B and layout-refined in Phase 5.5C.

## Folders

### `kinematics/`

Public-facing animations (GIF/MP4) illustrating joint-to-actuator motion for the
parallel-linkage leg joints:

- linkage motion
- joint-to-actuator mapping
- actuator extension/contraction
- coupled joint behavior

One subfolder per joint: `ankle/`, `knee/`, `thigh/`. A joint may have more than one
clip (e.g. additional viewpoints); currently each joint has a single combined
animation.

### `analysis/`

Public-facing figures for the Jacobian / determinant / workspace analysis behind the
same joints:

- Jacobian analysis
- determinant analysis
- singularity boundaries
- reachable / feasible regions
- actuator-limit constraints
- operating-region analysis

One subfolder per joint: `ankle/`, `knee/`, `thigh/`.

## Public-media constraint

These assets may be based on real engineering analysis, but public exports should
avoid disclosing exact production-specific values — e.g. prefer normalized axes,
generic configuration labels, normalized determinant/Jacobian quantities, and
qualitative actuator-limit or singularity boundaries over exact actuator strokes,
mechanism dimensions, or joint limits. This is guidance for what gets exported here,
not a legal disclaimer.

## Committed files (final, as of Phase 5.5C)

| File | Dimensions | Size |
|---|---|---|
| `kinematics/ankle/ankle_mapping.gif` | 800×1000 | ~1.24 MB |
| `kinematics/knee/knee_mapping.gif` | 800×1000 | ~485 KB |
| `kinematics/thigh/thigh_mapping.gif` | 800×1000 | ~352 KB |
| `analysis/ankle/ankle_determinant.png` | 1136×1485 | ~288 KB |
| `analysis/knee/knee_determinant.png` | 1185×1483 | ~122 KB |
| `analysis/thigh/thigh_determinant.png` | 1185×1483 | ~130 KB |

These are the final, manually reframed/cropped source assets — treat them as
authoritative; do not re-crop or regenerate. All six are referenced from the
Humanoid case study's "Kinematic Mapping & Operating-Range Analysis" subsection.
The three `analysis/*_determinant.png` figures link to their full-resolution file
on click. `ankle_mapping.gif` is the largest asset at ~1.24 MB — a future MP4/WebM
conversion would reduce this if page weight becomes a concern; no such conversion
has been done.

Note: a duplicate file (`kinematics/ankle/Thigh_Animation_Only.gif`, byte-identical
to `kinematics/thigh/thigh_mapping.gif`) was found misplaced in the ankle folder
during Phase 5.5C and removed — it was never referenced from `index.html`.

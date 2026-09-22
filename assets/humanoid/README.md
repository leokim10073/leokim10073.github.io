# Humanoid technical evidence — asset staging

Staging area for public-facing visual evidence supporting the Humanoid case study's
Kinematics & Real-Time Mapping section. No media is wired into `index.html` yet — this
structure exists so files can be organized ahead of the Phase 5.5B integration pass.

## Folders

### `kinematics/`

Public-facing animations (GIF/MP4) illustrating joint-to-actuator motion for the
parallel-linkage leg joints:

- linkage motion
- joint-to-actuator mapping
- actuator extension/contraction
- coupled joint behavior

One subfolder per joint: `ankle/`, `knee/`, `thigh/`. A joint may have more than one
clip (e.g. front and side views).

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

## Suggested filenames

```
assets/humanoid/kinematics/ankle/ankle_front.gif
assets/humanoid/kinematics/ankle/ankle_side.gif
assets/humanoid/kinematics/knee/knee_mapping.gif
assets/humanoid/kinematics/thigh/thigh_mapping.gif

assets/humanoid/analysis/ankle/ankle_determinant.png
assets/humanoid/analysis/knee/knee_determinant.png
assets/humanoid/analysis/thigh/thigh_determinant.png
```

These are naming suggestions only — no files currently exist in this structure
(confirmed: no local ankle/knee/thigh/determinant/kinematics media was found in the
working environment as of Phase 5.5A). Each subfolder currently holds only a
`.gitkeep` placeholder so the empty structure is tracked by git.

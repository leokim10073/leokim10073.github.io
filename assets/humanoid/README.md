# Humanoid technical evidence

Public-facing visual evidence supporting the Humanoid case study's Kinematics &
Real-Time Mapping section ("Kinematic Mapping & Operating-Range Analysis"), wired
into `index.html` as of Phase 5.5B.

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

## Committed files

```
assets/humanoid/kinematics/ankle/ankle_mapping.gif   (~1.79 MB)
assets/humanoid/kinematics/knee/knee_mapping.gif     (~350 KB)
assets/humanoid/kinematics/thigh/thigh_mapping.gif   (~278 KB)

assets/humanoid/analysis/ankle/ankle_determinant.png (~318 KB)
assets/humanoid/analysis/knee/knee_determinant.png   (~134 KB)
assets/humanoid/analysis/thigh/thigh_determinant.png (~138 KB)
```

All six files are referenced from the Humanoid case study's "Kinematic Mapping &
Operating-Range Analysis" subsection. The ankle determinant/knee/thigh figures link
to their full-resolution PNG on click. `ankle_mapping.gif` is the largest asset at
~1.8 MB — a future MP4/WebM conversion would reduce this if page weight becomes a
concern; no such conversion has been done yet.

The remaining empty leaf folders (if any) still hold a `.gitkeep` placeholder so the
directory structure stays tracked by git.

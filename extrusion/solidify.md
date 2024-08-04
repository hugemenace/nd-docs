# Solidify (<span title="Recallable">R</span>)

The Solidify operator will add thickness to any selected 2D or 3D object. It is well suited for turning a sketch or cross-section into workable 3D geometry.

[](../_media/solidify.mp4 ':include')

## Options

| Option | Shortcut | Mouse Value Compatible | Description |
| :--- | :--- | :--- | :--- |
| Thickness | _None_ | **Yes** | The thickness of the solidification |
| Offset | _None_ | **Yes** | The normal displacement of the solidification |
| Weighting | **`W`** | No | The weighting/direction of the solidification (positive, neutral, or negative) |
| Mode | **`M`** | No | Extrusion algorithm (see explanation below) |

## Alternative modes

Hold down the shortcut when selecting the operator to enter the respective mode.

| Shortcut | Description |
| :--- | :--- |
| **`CTRL`** | **RESET**: Remove any related modifiers from the selected object |

## Extrusion Algorithm (Mode)

### Simple
This is the default solidify algorithm, which simply extrudes the geometry. This algorithm does not work on geometry where edges have more than two adjacent faces.

### Complex
This is a solidify algorithm which can handle every geometric situation to guarantee a manifold output geometry. This algorithm is able to solidify shapes like Möbius strips, Klein bottles, architectural wall layouts and many more which the Simple Mode isn’t able to do. If the special cases are not present it is recommended to choose Simple because the extra logic makes this algorithm much slower.

Read the full description at the [official Blender documentation](https://docs.blender.org/manual/en/latest/modeling/modifiers/generate/solidify.html).
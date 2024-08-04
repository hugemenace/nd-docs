# Edge Bevel (<span title="Recallable">R</span>)

The Edge Bevel operator will perform a edge specific bevel, allowing you to customise the width, segments, and profile.

?> **Note:** the edge bevel operator allows you non-destructive apply bevels to individual edges, however, the options for width, segments, profile, and harden normals are applied to all edge-bevels on the selected object and cannot be controlled at an individual edge level. This is simply a limitation of the built-in bevel modifier in Blender.

[](../_media/edge-bevel.mp4 ':include')

## Options

| Option | Shortcut | Mouse Value Compatible | Description |
| :--- | :--- | :--- | :--- |
| Weight | _None_ | **Yes** | The weight (width factor) of the bevel |
| Segments | _None_ | **Yes** | The number of segments (sides) |
| Profile | _None_ | **Yes** | The profile of the bevel (concave, convex, neutral) |
| Width | _None_ | **Yes** | The width of the bevel |
| Clamp Overlap | **`C`** | No | Clamp the width to avoid overlap |
| Loop Slide | **`S`** | No | Prefer sliding along edges to having even widths |
| Harden Normals | **`H`** | No | Wether to enable hardened normals |

## Alternative modes

Hold down the shortcut when selecting the operator to enter the respective mode.

| Shortcut | Description |
| :--- | :--- |
| **`SHIFT`** | Place modifier at the top of the stack |
| **`CTRL`** | **RESET**: Remove any related modifiers from the selected object |
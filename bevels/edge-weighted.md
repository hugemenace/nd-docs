# Edge Weighted Bevel (<span title="Recallable">R</span>)

The Edge Weighted Bevel operator will perform an edge specific bevel, allowing you to customise the width, segments, and profile.

?> **Note:** the edge weighted bevel operator allows you to apply non-destructive bevels to individual edges, however, the options for width, segments, profile, and harden normals are applied to **all** edge-bevels on the selected object and cannot be controlled at an individual edge level. For multiple unique edge bevels on the same object, use the [Edge Attribute Bevel](/bevels/edge-attribute) operator.

## Options

| Option | Shortcut | Mouse Value Compatible | Description |
| :--- | :--- | :--- | :--- |
| Width | _None_ | **Yes** | The width of the bevel |
| Segments | _None_ | **Yes** | The number of segments (sides) |
| Profile | _None_ | **Yes** | The profile of the bevel (concave, convex, neutral) |
| Weight | _None_ | **Yes** | The weight (width factor) of the bevel |
| Width Type | **`W`** | No | The width type (offset, width, depth, percent, absolute) |
| Harden Normals | **`H`** | No | Whether to enable hardened normals |
| Enhanced Wireframe | **`E`** | No | Display the object's wireframe over solid shading |
| Clamp Overlap | **`C`** | No | Clamp the width to avoid overlap |
| Loop Slide | **`S`** | No | Prefer sliding along edges to having even widths |


## Alternative modes

Hold down the shortcut when selecting the operator to enter the respective mode.

| Shortcut | Description |
| :--- | :--- |
| **`SHIFT`** | Place modifier at the top of the stack |
| **`CTRL`** | **RESET**: Remove any related modifiers from the selected object |
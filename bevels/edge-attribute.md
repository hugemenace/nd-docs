# Edge Attribute Bevel (<span title="Recallable">R</span>)

The Edge Attribute Bevel operator will perform an edge specific bevel at an individual edge level based on object data attributes, allowing you to customise the width, segments, and profile. This allows for multiple unique edge bevels on the same object.

!> **Compatibility:** Blender 4.3 and above.

## Options

| Option | Shortcut | Mouse Value Compatible | Description |
| :--- | :--- | :--- | :--- |
| Width | _None_ | **Yes** | The width of the bevel |
| Segments | _None_ | **Yes** | The number of segments (sides) |
| Profile | _None_ | **Yes** | The profile of the bevel (concave, convex, neutral) |
| Width Type | **`W`** | No | The width type of the bevel (offset, width, depth, percent, absolute) |
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
# Preferences

## General

| Setting | Description |
| --- | --- |
| **Utils Collection Name** | The name of the automatically created collection where all util objects are placed |
| **Use Fast Booleans** | Whether to use the "FAST" solver option on boolean modifiers, or the "EXACT" solver option |
| **Automatically run Solidify after Recon Poly** | When enabled, will automatically invoke the Solidify operator after finishing a Recon Poly operation |
| **Automatically set Recon Poly extents to Inscribed (vs. Circumscribed)** | When enabled, will set the default extents mode for Recon Poly to "Inscribed" |
| **Bevel / Smooth Angle** | The default angle to use for bevel and smoothing operations (30, 45, or 60 degrees) |
| **Custom Screw Heads** | A path to a custom `.blend` file containing screw heads to be used in addition to the default set provided by the [Screw Head Operator](/standalone/screw-head) |
| **Enable Update Checks** | Will automatically check if a new version of the addon is available when Blender starts |
| **Compatibility Mode** | Whether to show deprecated (legacy) features in the UI |

## UI

| Setting | Description |
| --- | --- |
| **Overlay DPI** | The DPI (size) of the overlay UI |
| **Enable Mouse Values** | Whether to enable mouse values mode (i.e. increasing or decreasing the value of the selected operator option by moving the mouse) |
| **Lock Overlay Pinning** | Whether to remember the overlay UI's position when it is pinned |
| **Enable Axis Visualization** | Whether to show the axis visualiser when using operators that have an axis option |
| **Axis Base Thickness** | The base thickness of the axis visualiser |
| **Axis Active Thickness** | The thickness of the active (selected) axis |
| **Axis Inactive Opacity** | The opacity of the inactive (unselected) axes |
| **Custom Overlay Options** | Select which overlays will be kept on when toggling the 3D viewport overlays, see below. |

?> **Custom viewport overlay options:** `show_annotation`, `show_axis_x`, `show_axis_y`, `show_axis_z`, `show_bones`, `show_cursor`, `show_extras`, `show_floor`, `show_motion_paths`, `show_object_origins`, `show_object_origins_all`, `show_ortho_grid`, `show_outline_selected`, `show_relationship_lines`, `show_stats`, and `show_text`.

## Keymap

Contains the keymap for all of the customisable addon [shortcuts](/getting-started/shortcuts).

## Theme

Contains customisable theme color settings for the addon, and the option to revert back to the default theme.
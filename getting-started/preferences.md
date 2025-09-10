# Preferences

## General

| Setting | Description |
| --- | --- |
| **Use Fast Booleans** | Whether ND will use the _Fast/Float_ solver option on boolean modifiers or the _Exact_ solver option |
| **Create Custom Transform Orientations with View Align** | Whether ND will save a custom transform orientation (i.e. alongside global, local) when using View Align  |
| **Enable Right Click Select** | Alter ND's behaviour so that it is more compatible with right-click select in Blender |
| **Enable Auto Smoothing** | Whether ND will automatically add auto smoothing to objects after performing various operations |
| **Bevel / Smooth Angle** | The default angle to use for bevel and smoothing operations (30, 45, or 60 degrees) |
| **Enable Update Checks** | Will automatically check if a new version of the addon is available when Blender starts (only available when ND is installed from disk) |
| **Utils Toggle Behaviour** | Whether ND will use the _Disable in Viewports_ or _Hide in Viewport_ behaviour when toggling util visibility.
| **Experimental Mode** | Enable experimental features. Use at your own risk! |

## UI

| Setting | Description |
| --- | --- |
| **Overlay DPI** | The DPI (size) of the ND overlay UI |
| **Enable Mouse Values** | Whether to enable mouse values mode (i.e. increasing or decreasing the value of the selected operator option by moving the mouse) |
| **Extend Mouse Values** | Whether to enable extended mouse values. This mode will allow you to change the segments on bevel using the scroll wheel without having to hold down the ALT key |
| **Mouse Value Scalar** | A scalar value to apply to raw mouse delta when using mouse-driven values. Useful to avoid harsh or massive value changes with small mouse movements. |
| **Mouse Value Steps** | Determines how far the mouse needs to move to register one "step" — utilised for parameters such as count, segments, etc. |
| **Unit Increment Size** | The size of each unit increment; used for value changes with the mouse scroll wheel or up and down arrow keys. |
| **Enable Quick Favourites** | This option will show Blender's quick favourites menu at the end of the main ND menu. Useful when rebinding ND's main menu shortcut to the Q key |
| **Lock Overlay Pinning** | Whether to remember the overlay UI's position when it is pinned |
| **Lock Overlay Parameters on Recall** | When enabled, will cause ND to lock all parameters when an operator is recalled. This helps prevent accidental value changes when Mouse Values is enabled |
| **Enable the sidebar** | Whether to show the N-panel sidebar (requires a Blender restart after changing this setting) |
| **Enable Axis Visualization** | Whether to show the axis visualizer when using operators that have an axis option |
| **Axis Base Thickness** | The base thickness of the axis visualizer |
| **Axis Active Thickness** | The thickness of the active (selected) axis |
| **Axis Inactive Opacity** | The opacity of the inactive (unselected) axes |
| **Hide Asset Library Install Prompt** | Prevents the install prompt from showing in ND's N-Panel menu |
| **Custom Overlay Options** | Select which overlays will be kept on when toggling the 3D viewport overlays; see below. |

?> **Custom viewport overlay options:** `show_annotations`, `show_axis_x`, `show_axis_y`, `show_axis_z`, `show_bones`, `show_cursor`, `show_extras`, `show_floor`, `show_motion_paths`, `show_object_origins`, `show_object_origins_all`, `show_ortho_grid`, `show_outline_selected`, `show_relationship_lines`, `show_stats`, and `show_text`.

## Keymap

Contains the keymap for all of the customisable addon [shortcuts](/getting-started/shortcuts).

## Theme

Contains customisable theme color settings for the addon, and the option to revert to the default theme.
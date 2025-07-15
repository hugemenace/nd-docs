# Changelog

## 1.48.0 (2025-02-19)


## Features

* add a 'Boolean Connectors' option to the GN Pipe Generator modifier
* add the new Generators menu to the N-Panel on Blender 4.3+

## Bug Fixes

* ensure the Generators shortcut menu (Shift Alt G) is not bound on Blender versions lower than 4.3
* fix the Pipe Generator error when corner mode is activated on an edge with less than 3 vertices

## 1.47.0 (2025-02-11)


### Features

* add edge length operator
* add GN hole generator
* add GN pipe generator
* add the pipe generator operator to the fast menu replacing pipe extrude


### Bug Fixes

* fix the Flare energy offset parameter reset after energy levels have been randomised

## 1.46.0 (2024-11-23)


### Features

* add an option to disable the creation of a custom transform orientation when using view align
* add an option to disable util viewport visibility when toggling (in addition to hiding)
* add an option to stop ND from hiding all unrelated utils when an operation creates or recalls another util object
* set the material mode on exact booleans to transfer


### Bug Fixes

* ensure that util objects aren't rendered when in Cycles or EEVEE preview modes
* ensure that utils aren't relocated to the root of the utils collection if they already exist in a sub-collection
* ensure the panel operator's BMesh instance is not prematurely freed during operation
* ensure the utils collection is included in the current view layer when utils are created or recalled
* move the vertices/edges selected polling methods into the invoke method for the edge_bevel, vertex_bevel, and clear_vgs operators to avoid freeing any existing object's BMesh instance

## 1.45.0 (2024-08-04)


### Features

* add duplicate utility operator and corresponding fast menu integration
* add pipe extrude operator and corresponding fast menu integration
* add the option to clear/remove drivers (and retain existing values) to the sync modifiers operator
* improve sync modifiers attribute detection and add support for geometry nodes
* mark sync modifiers as a standard feature (previously experimental)
* retain original object and offset_object utils when syncing modifiers and add an option to override (ALT) if required


### Bug Fixes

* fix maximum recursion depth exceeded error when smart duplicating an object with cylic utils
* fix the error that occurs when cancelling a panel operation on the first step (selecting geometry)

### 1.44.3 (2024-07-20)


### Bug Fixes

* ensure that only one triangulate modifier is applied to an object when running the operator multiple times
* ensure the triangulate modifier is placed/pinned at the end of the mod stack
* ensure the triangulate modifier is removed from boolean utility objects
* improve F2 add-on/extension detection and subsequent Fast menu "Make Edge/Face" prediction
* improve operator polling and the edit mode predictions in the Fast menu

### 1.44.2 (2024-07-13)


### Bug Fixes

* ensure all bmesh instances are freed after use to prevent memory leaks
* fix ND N-panel toggle-utils shortcut icon registration error

### 1.44.1 (2024-07-12)


### Bug Fixes

* fix Blender version polling

## 1.44.0 (2024-07-12)


### Features

* add a linked version of smart duplicate (equivalent to Blender's ALT + D)
* add extended mouse behaviour support (scroll on bevels to change segment count)
* add extended mouse value support to recon poly (scroll to adjust segments)
* add freeze state option to modifier mode in the cycle operator (retain mod visibility states on exit)
* add mirror, profile extrude, and screw operators to the edit mode fast menu
* add option to change overlay reset key behaviour to unlock instead of hard-reset
* add option to customise the Utils collection icon color
* add option to lock overlay parameters on recall
* add option to remove triangulate modifiers via the CTRL alt-mode convention
* add SHIFT+T shortcut for toggle utils
* add smart duplicate operator (copy selected object/s with all associated utilities)
* add symmetrize option to mirror operator for immediate application
* add sync modifiers operator (experimental feature)
* allow apply modifiers to be run on curve objects in selection set (will convert them to mesh)
* allow bulk operators to be executed as long as mesh objects are in the selected group (e.g., ignore empties)
* allow profile extrude, screw, mirror, and circularize operators to be run from edit mode
* allow the isolated object util toggle operator to be run on composite utils


### Bug Fixes

* ensure that all util objects are toggled (including empties) when using the isolated object mode in toggle utils
* ensure that all utils and composited utils are recursively selected when toggling or duplicating
* fix Blender 4.2 SBA crash and improve SBA/WN across various versions
* only attempt to preserve custom normals when running triangulate in Blender <4.2

### 1.43.1 (2024-06-12)

## 1.43.0 (2024-06-03)


### Features

* add an option in general preferences to toggle auto smoothing across all operators


### Bug Fixes

* fix version number check when check for updates is enabled

## 1.42.0 (2024-05-25)


### Features

* add a hard apply & duplicate mesh alternative mode to the apply modifiers operator


### Bug Fixes

* fix the incorrect object position offset when reversing a faux origin displacement

### 1.41.2 (2024-05-08)

### 1.41.1 (2024-05-07)


### Bug Fixes

* fix Blender 4.2 extension compatibility issues

## 1.41.0 (2024-04-15)


### Features

* add an option to toggle the visibility of utils for only the selected objects
* add robertson, torx tamper proof, and triangle recess screw head types


### Bug Fixes

* ensure that boolean ops handle the presence of WN mods correctly
* ensure that the SBA and WN mod order is maintained when new mods are added to the stack
* ensure that the WN modifier doesn't add additional mods to an object with the WN mod already applied
* ensure the SBA mod places itself before any WN mod present in the stack
* fix NoneType error and add additional guard clauses for when the active target object is excluded from the view layer
* fix smoothing mod removal error on profile extrude when cancelling a new (non-recalled) operation

## 1.40.0 (2024-03-22)


### Features

* add right-click select support (toggle via add-on preferences)
* add support for Blender 4.1's new smoothing process


### Bug Fixes

* fix circular array empty rotation in single-object mode and tidy up operator
* fix lattice scaling in Blender >= 4.1

## 1.39.0 (2024-02-03)


### Features

* add the option to stack bevel modifiers, and cycle through stacked bevels when recalling


### Bug Fixes

* ensure that the edge.index exists in the edges_snapshot before reverting an edge bevel operation

## 1.38.0 (2023-12-01)


### Bug Fixes

* fix additional Blender 4 compatibility issues
* fix Blender 4 compatibility issues
* fix Blender 4 shader issues for Axis and Point visualisation

## 1.37.0 (2023-07-14)


### Features

* add an apply modifier option to the cycle operator
* add keymaps for difference, union, intersect, and slice boolean operations
* add loop slide and clamp overlap options to the edge bevel modifier and swap the weight and width options
* add only ngons option to triangulate modifier
* add support to high/low LOD for ZenSet's object naming convention
* remove the WN bevel operator and update the standard bevel and weighted normal operators so that the functionality can be replicated
* set the angle parameter on the bevel operator as a mouse-driven value


### Bug Fixes

* fix the edge bevel operator's width and weight hints

### 1.36.1 (2023-02-06)


### Bug Fixes

* fix error in panel operator after geometry selection

## 1.36.0 (2023-01-31)


### Features

* add adaptive unit fallback support for both metric (meters) and imperial (feet)
* add constant displacement mode option to array_cubed operator
* add full support for Blenders unit system (None, Metric, and Imperial) and unit scales
* add mouse-value support to all non-keybound operator options
* add scene unit scale support for operator overlay values
* add silhouette operator


### Bug Fixes

* add fallback support for Blender's "Adaptive" unit length (default to meters)
* ensure object names with multiple chained ".00n" suffixes are fixed before high and low LOD naming operations
* fix screw head z-axis displacement issue when altering scale
* fix XYZ axis visualisation extents
* set weld mode to connected for all bevel operators

## 1.35.0 (2022-11-05)


### Features

* add circularize operator
* add clamp_overlap and loop_slide options to bevel operator
* add decimate modifier to circularize operator and set min segments to 2
* add immediate apply mode to seams operator, default to angle set in preferences, and lock auto smooth to 180 degrees
* add mesh mode set_origin behaviour
* add the circularize operator as a fast menu PE/sketch prediction


### Bug Fixes

* add edge_bevel and overlay fixes for Blender 3.4
* add overlay_option_active_color back into reset_theme operator
* ensure vertex groups and edge weights are remove when applying modifiers
* fix profile_extrude and solidify normal calculations
* only apply viewport visible modifiers
* register recon_poly segments with mouse values system

## 1.34.0 (2022-09-19)


### Features

* add a bulk assign ID materials operator
* add a weighted_normal operator along with a new shading category, and move smooth shading into it
* add clean_utils and apply_modifiers ops as shortcuts in main UI panel
* add clear_materials operator
* add CTRL + click modifier removal behaviour to all applicable operators
* add experimental mode toggle to preferences
* add mirror operation to boolean object fast menu predictions
* add mouse-step values to lattice, screw, array_cubed, circular_array operators
* add Shift + Alt + E keybinding for the Packaging menu
* add smooth shading and weighted normal operators to the fast-predict menu
* add the id_material operator
* add undo/redo/W/C event passthrough as experimental feature for geo_lift, panel, and view_align operators
* allow bevel segments to be set via mouse movement when mouse values are enabled
* allow customisation of the overlay base color
* allow ID Materials to be actioned in both object and edit mode (face select)
* allow smooth shading operator to be used on multiple objects simultaneously
* create a dedicated ID materials menu under Packaging, and a new assign-existing ID material operator
* remove edge weights and vertex groups when clearing edge_bevel, or vertex_bevel operations
* set keep_sharp for the weighted_normal operator by default
* split applicable util ops into dedicated scene and export menus
* update the ID Materials menu to show a static list of all available colours with previews


### Bug Fixes

* ensure mod order is rectified when using the edge_bevel operator
* ensure select objects are made single-user when executing the apply_modifiers operator
* explicitly import bpy.utils.previews in icons/__init__.py
* fix array_cubed manual input override locking
* set profile_extrude's calculate edges option to false by default

## 1.33.0 (2022-08-06)


### Features

* add clear scale and shrink/fatten to sketch menu for object and edit mode respectively
* add curve support to array_cubed operator
* add curve support to screw operator
* add curve support to simple_deform operator
* add mirror curve option to fast predict menu
* add option to mirror curve(s)
* add screw, array_cubed, and simple_deform curve operators to fast predict menu
* add toggleable exclusive view (x-ray option) option to geo_lift, panel, and view_align operators
* split clear_view into overlay (all & custom) options


### Bug Fixes

* ensure make edge/face operation is always available in edit mode fast menu
* ensure weld modifier removal does not prevent standard bevels from being recalled, and avoid removing HN bevel welds during apply-modifier operations
* fix lattice target object parenting behaviour
* fix the "no predictions found" edge case in the Fast menu with only surfacing recallable operators
* set width lower limit to zero on WN bevel operator

## 1.32.0 (2022-06-25)


### Features

* add an option to toggle the sidebar / N-panel
* add calculate edges option to profile_extrude operator
* add extrusion mode option to solidify operator
* add interpolation mode to lattice operator and default to linear
* add offset option to profile_extrude operator
* add solidify option to fast menu for non-manifold meshes
* add the ability to recall previous edge bevel weights
* add toggle wireframe and disable utility modifier options to cycle operator
* enhance profile extrusion and solidification predictions in the Fast menu
* ensure mirror modifiers are placed before finishing bevels in the modifier stack
* rectify the mod order for lattice, simple_deform, profile_extrude, screw, solidify, array_cubed, and circular_array operators
* remove all disabled (viewport hidden) boolean modifiers when using the clean_utils operator


### Bug Fixes

* add missing fast menu no prediction results section count
* add missing new_modifier imports to recon_poly, screw_head, set_origin, and triangulate operators
* ensure single_vertex object has rotation and scale applied after creation
* fix edge_bevel width shift/precision and value formatting
* fix error/crash in clean_utils utility & add logic for lattice modifiers
* fix mesh_f2 addon detection in the Fast Predict menu
* fix no predictions logic in the fast menu
* fix poll method target object type check in cycle operator
* handle object/modifier removal errors more gracefully in clean_utils operator
* unify and lower the merge and bisect thresholds for the mirror operator

## 1.31.0 (2022-06-12)


### Features

* add clean geometry logic to view align, and allow view align to be immediately invoked on applicable geometry with an alt mode
* add collapsible sections and common shortcuts to the N panel menu
* add inscribed and circumscribed options to recon_poly operator
* add the panel, geo_lift, and view_align operators to fast menu single object form predictions
* automatically collapse new modifiers added to objects
* extend inscribed and circumscribed feature to recon_poly inner_radius option & fix recall/revert behaviour
* remove problematic bevels from all boolean reference objects


### Bug Fixes

* ensure viewport camera is always set to orthographic when using view_align operator
* fix array_cubed count reset behaviour while respecting the currently specified offset value
* fix direct object view_align operation when utilising edges or vertices
* fix mirror across geometry behaviour and unneeded show_in_front assignment for evaluated geometry
* fix up single and multi-object geometry mirror object evaluation and empty parenting

## 1.30.0 (2022-06-06)


### Features

* add additional screw head types (@Shaddow)
* add better boolean and sketch detection in the fast prediction menu
* add clean_utils operator
* perform additional geometry cleanup when extracting faces using the panel operator


### Bug Fixes

* ensure boolean swap_solver updates only apply to objects referencing the selected utils
* ensure clean_utils also handles mirror and array empty objects in utils collection
* ensure that individual faces cannot be toggled until the inset stage in the panel operator
* fix create_duplicate_liftable_geometry object_name parameter being overridden
* fix error when using swap solver on a utility referenced by an object with invalid boolean modifiers present
* fix NoneType object error when cycling through a utility object

## 1.29.0 (2022-06-02)


### Features

* add hard-apply mode to apply_modifiers utility, and exclude regular multi segment edge bevels from normal usage
* add mirror operator to the fast menu for profile predictions
* add ND theme (color) options to preferences
* add panel operator
* add recon poly detection to fast menu
* add remaining boolean operations to the fast menu
* add shift alt-mode to set_origin utility to undo faux origin translations
* add solidify and profile extrude options to the fast menu when operators have been previously performed on the selected object
* clean up duplicated mesh by default when using geo_lift or panel operators, with option to preserve geometry
* detect additional existing mods in fast menu
* ensure starting geometry is reselected when reverting geo_lift operator
* harden up circular_array operator, add displacement axis option, and regular/faux origin alt mode


### Bug Fixes

* add an additional clause to the circular_array poll method
* add missing continue statements in create_duplicate_liftable_geometry
* ensure the inset stage only begins if one or more faces have been selected when using the panel operator
* ensure the reference object origin is restored when cancelling a new circular array operation
* fix mod reference error in create_duplicate_liftable_geometry function in object library
* fix profile extrude recall and revert behaviour
* fix recon poly local Z axis natural rotation and recall ability
* tidy up and fix undesired relative offset behaviour in panel operator

### 1.28.4 (2022-05-28)


### Bug Fixes

* add additional checks to bevel types in automatic modifier reordering logic

### 1.28.3 (2022-05-28)


### Bug Fixes

* fix modifier stack ordering when vertex bevel + weld modifiers are present

### 1.28.2 (2022-05-27)

### 1.28.1 (2022-05-27)


### Bug Fixes

* fix unexpected float error in Blender 3.1 and limit the possibility of dividing by zero errors on manual user input

## 1.28.0 (2022-05-27)


### Features

* add alt mode to vertex bevel to create a vertex group edge bevel
* add an option to custom default smoothing angle and update & add it across all relevant operators
* add apply_modifiers utility
* add cycle operator to fast menu for objects with boolean modifiers present
* add decimate and weld operators under the new simplify menu
* add edge angle limit option to bevel and weight_normal_bevel operators
* add enhanced wireframe mode toggle to all bevel operators
* add fast prediction menu
* add flip normals option to screw operator
* add natural rotation option to recon poly
* add option to place modifiers at the top/bottom of the stack across edge_bevel, vertex_bevel, and mirror
* add swap_solver utility
* add the option to disable automatic update checks in preferences
* allow for manual values to be supplied to overlay & optimise operator overlay options
* allow hydrate utility to be run on multiple selected objects
* automatically move booleans under WN bevels and single segment HN bevels
* bind the fast menu to F and add a shortcut for Blender's underlying make edge/face operator
* improve the mod ordering logic and apply it to the weld and decimate modifiers


### Bug Fixes

* add a check to apply_modifiers for disabled modifiers and remove them instead of applying
* add missing draw_hint import to edge_bevel operator
* display no prediction message when in edit mode and no precondition matches
* fix up has_mod_* logic in fast menu single object predictions
* fix weighting calculation in profile_extrude operator
* remove triangulate modifier & switch v3_average for .calc_center_median for face points in snap_align operator

## 1.27.0 (2022-05-14)


### Features

* add Flare (Lighting) operator
* add option to automatically run solidify after a recon poly operation
* add option to capture 2 points in snap_align to align the selected object at the midpoint
* add recall ability to circular_array operator
* add snap_align operator
* add temporary triangulation to active object during snap_align operations to increase face points
* allow circular_array operator to be used on a single selected object, and alter origin/translation logic
* allow snapping to occur through objects occluding the target while using snap_align
* enhance lattice modifier behaviour and allow it to be recalled
* hide circular_array empties on completion and give them an appropriate name


### Bug Fixes

* ensure active boolean utils don't affect the geometry of the target object while using snap_align
* ensure guideline in snap_align operator is cleared when capture rotation is reset
* ensure mirror selected object show_in_front mode is disabled on complete/cancel
* ensure simple deform angle decrements as intended using the step_down key event
* ensure snap_align operator supports meshes with vastly different edge lengths
* ensure that the reference object is solo-selected when completing a snap_align operation
* fix circular array revert behaviour for single object mode
* fix error when using cycle operator on objects with objectless booleans in their modifier stack
* fix left-click handling for operators that need to pass through the event
* fix mirror over geometry empty's matrix parent inverse
* fix up circular_array and lattice overlay option control key labels
* only detect click events on release when using interactive operators
* remove light energy offset limits

## 1.26.0 (2022-05-07)


### Features

* add enter & space key presses as additional operator finalisation events
* add modifier & utility cycle operator
* add option to mirror across faces, edges, or vertices on selected object
* add shift option to vanilla boolean operator to protect reference object (do not convert into utility)
* add simple_deform operator
* add triangulate modifier
* allow for multiple utils to be selected with cycle operator
* allow mirror modifier to be applied to multiple objects simultaneously
* automatically set geometry mirror axis to Z and flipped
* move sketch operators into their own sub-menu
* tidy up main menu by creating Replication and Deformation sub menus to house appropriate operators


### Bug Fixes

* ensure boolean operators isolate the reference object in the utils collection
* ensure mirror empty object is removed if mirror operator is cancelled after geometry selection
* fix alt key value change behaviour on cycle operator
* fix geo_lift operator event handling order
* fix recon poly width option overlay display value
* fix reference/target object parenting in circular_array operator
* fix up mirror across geometry invalid selection cleanup logic
* update set_lod_suffix mode type in utils_menu

## 1.25.0 (2022-04-29)


### Features

* add clear vertex groups utility
* add isolated vertices in selection to active group in vertex bevel recall
* add recall functionality to vertex bevel operator
* add shortcut for isolated utils menu


### Bug Fixes

* fix circular array revert behaviour
* match target object rotation in circular_array operator
* remove set rotation from faux set_origin
* replace center of volume with bounding box calculation in lattice operator

## 1.24.0 (2022-04-26)


### Features

* add alt mode to geo_lift operator to ignore all bevels when calculating selectable geometry
* add bool_inset operator
* add edge_bevel operator
* add harden normals option to vanilla bevel operator
* add lattice operator
* add mode option shortcut key for bool_inset operator
* add option to lock overlay pin state and position across all operators
* add outset mode to bool_inset operator
* add toggle option shortcut keys to applicable operators
* add traditional (now default) and faux origin translation to set_origin utility
* allow for -360 degree rotation on screw operator
* set face strength mode and face influence on wn_bevel modifiers


### Bug Fixes

* add additional checks to all operator poll methods to avoid selection (and order) based errors
* ensure circular_array operator allows for traditional (now default) and faux origin translation
* remove all ND menus from info header bar
* set miter_outer to arc in bevel operator

## 1.23.0 (2022-04-22)


### Features

* allow array_cubed count to roll faux negative
* distinguish between built-in and custom screw head types in the operator overlay, and add additional .blend file cleanup on revert

## 1.22.0 (2022-04-22)


### Features

* add array_cubed operator and deprecate square_array
* add custom screw heads (.blend file) option to addon preferences
* add enhanced axis visualization to array_cubed, mirror, profile_extrude, and screw modifiers
* add toggle for "fast" booleans in addon preferences and set default to true (previously "exact")
* allow circular_array operator to be run on objects, empties, and at arbitrary rotations
* show axes on selected object when using the array_cubed operator


### Bug Fixes

* match target object rotation in set_origin operator

## 1.21.0 (2022-04-18)


### Features

* add mouse values mode, and integrate all applicable operators
* add profile option to vanilla bevel operator


### Bug Fixes

* ensure a weld modifier is placed after a vanilla bevel modifier
* ensure the previous profile value is retained when summoning & reverting a vanilla bevel operator
* fix profile option behaviour on vertex_bevel operator
* swap width and segments options on vertex_bevel operator to align with vanilla bevel operator
* update recon_poly option ordering to better align with other operators (width > segments > etc.)

### 1.20.1 (2022-04-17)


### Bug Fixes

* ensure all scene objects are deselected before executing core single_vertex operator functionality

## 1.20.0 (2022-04-17)


### Features

* allow customization of overlay pin and pause keybinds
* organise addon preferences panel and expose Blender keymap settings
* split blank_sketch into single_vertex and make_manifold operators


### Bug Fixes

* fix incorrectly labled profile_extrude overlay alt/ctrl key options

## 1.19.0 (2022-04-12)


### Features

* add hydrate operator
* add option to enable quick favourites on primary menu
* add optional late-invocation mode to vertex bevel operator (for post-sketch usage)
* add ortho_grid to toggle_clear_view operator
* add viewport menu (with various initial toggles)
* automatically place boolean reference and circular array rotator objects in a utils collection (name configurable in preferences)


### Bug Fixes

* ensure all objects in utils collection are toggled along with the collection consistently
* fix object visibility error in toggle_utils_collection operator

## 1.18.0 (2022-04-09)


### Features

* add square_array operator and create arrays sub-menu
* allow active overlay values to be updated with arrow and WASD keys


### Bug Fixes

* ensure ND keymap is included in 3D View, Mesh, and Object Mode by default

## 1.17.0 (2022-04-05)


### Features

* add a message/button to the shortcut menu & a link to the changelog in the UI panel when an update is available
* add bevel operator
* add circular_array operator
* adjust circular array option order, add even/odd count step, and allow negative arc angles
* ensure mirror modifier bisects selected axis & add flip option for negative axis mirroring
* organise operators by relevance in the shortcut menu
* update documentation section on main UI panel & add Discord link


### Bug Fixes

* ensure operate is only executed on interactive option mutation

## 1.16.0 (2022-04-03)


### Features

* add overlay DPI control to preferences


### Bug Fixes

* ensure overlay option precision mode indicator is inactive when in pause mode
* ensure that the screw operator calculates the order of edges for correct normals

## 1.15.0 (2022-04-02)


### Features

* add manifold option to blank_sketch operator
* add profile_extrude operator


### Bug Fixes

* ensure solidify modifier uses even offset

## 1.14.0 (2022-04-01)


### Features

* add mirror operator
* automatically select and set active the boolean reference object


### Bug Fixes

* ensure that parented objects in all boolean operations have their transforms maintained

## 1.13.0 (2022-04-01)


### Features

* rename ring_and_bolt to recon_poly (regular convex polygon) as it more accurately represents its behaviour

## 1.12.0 (2022-03-31)


### Features

* add boolean slice operator
* ensure reference and secondary objects in boolean operations are parented to the primary object
* prefix boolean reference object names

### 1.11.2 (2022-03-30)


### Bug Fixes

* ensure ESC key does not cancel paused operators

### 1.11.1 (2022-03-30)

## 1.11.0 (2022-03-29)


### Features

* add the 3 core boolean operators, difference, union, and intersect


### Bug Fixes

* swap origin and destination objects in set_origin operator

## 1.10.0 (2022-03-27)


### Features

* add version detection, "update available" notification, and Gumroad link to main UI panel


### Bug Fixes

* fix erroneous unregister_draw_handler calls in screw, solidify, seams, and smooth operators

## 1.9.0 (2022-03-27)


### Features

* replace overlay fixed pin location with pin-in-place functionality


### Bug Fixes

* ensure seams operator turns on object auto smooth if override is set
* fix screw operator summon & revert error

## 1.8.0 (2022-03-26)


### Features

* add interactive UV seams & sharps operator

### 1.7.1 (2022-02-25)


### Bug Fixes

* ensure the decimate modifier retains its appropriate position in the stack when recalling the ring_and_bolt operator

## 1.7.0 (2022-02-19)


### Features

* add smooth operator


### Bug Fixes

* ensure vertex_bevel operator always places current bevel modifier at the top of the stack, and only creates one weld modifier in total

### 1.6.1 (2022-02-18)


### Bug Fixes

* reduce remove double vertices threshold in blank_sketch operator
* update scale parameter overlay representation in screw_head operator

## 1.6.0 (2022-02-08)


### Features

* add 3 point view-plane creation via vertex select mode in view_align operator
* add profile parameter to vertex bevel
* add set_origin utility operator
* add summon behaviour to screw, solidify, and wn_bevel operators
* add summon feature to ring_and_bolt operator
* split face_sketch operator into geo_lift and view_align, with improvements in each respectively


### Bug Fixes

* add vert, edge, face specific selection mode to geo_lift operator
* ensure all target geometry is deselected when first entering geo_lift, or view_align operators
* ensure cancel keybind cancels all operators, particularily while in halt mode
* ensure correct leftover geometry is removed based on selection mode in geo_lift operator
* ensure summoned ring_and_bolt operator reverts back to previous values on cancel
* fix solidify operator weighting label array index error
* remove unneeded viewport cursor wrap behaviour

## 1.5.0 (2022-02-06)


### Features

* add screw head generator
* add toggleable "halt" mode to all operators, allowing event / keybinding passthrough


### Bug Fixes

* add planar decimate modifier to ring_and_bolt objects if the segment count is greater than 3

## 1.4.0 (2022-02-04)


### Features

* add utils menu as sub-menu on main menu

## 1.3.0 (2022-01-31)


### Features

* add a dynamic relationship between inner radius and width parameters, for more predictive results, and better ring generation


### Bug Fixes

* enforce 0.0001 minimum width for weighted normal bevel, and add WN prefix to bevel modifier name for better recognition

### 1.2.1 (2022-01-30)


### Bug Fixes

* fix broken keymap entry property name for main menu after name change
* use more reliable collection objects link call for operators creating single vertex objects

## 1.2.0 (2022-01-30)


### Features

* add name_sync operator and new ND Utils UI panel
* add set_lod_suffix operator
* allow F key passthrough on face_sketch operator


### Bug Fixes

* clear custom split normals on extracted faces in face_sketch operator
* ensure clean up method in face_sketch operator removes extracted face when the operation is cancelled
* fix incorrect class name unregister call in main_menu.py
* fix poll method qualifier in name_sync operator
* set the bevel modifier offset type to 'width' for the vertex_bevel, and weighted_normal_bevel operators

### 1.1.1 (2022-01-29)


### Bug Fixes

* add missing capture_modifier_keys function call to invoke method on face_sketch operator
* remove hardcoded mm suffix on all operator overlay parameter labels
* set starting width parameter to 0 on vertex_bevel operator

## 1.1.0 (2022-01-29)


### Features

* add face extraction mode to view_align operator and rename it to face_sketch, rename new_sketch to blank_sketch, and sketch_bevel to vertex_bevel
* rename operators - spinner to screw, thickener to solidfiy, and faux_bevel to weighted_normal_bevel
* split offset and thickness modifiers from bolt operator in favour of solidy operator usage, add ring functionality to bolt operator, rename bolt to ring_and_bolt


### Bug Fixes

* add invalid face selection error handling for face_sketch operator
* ensure update_overlay function is called after every event type
* fix ring_and_bolt parameters and parameter names to more appropriately represent their behaviour
* update solidify weighting parameter name

## 1.0.0 (2022-01-28)


### Features

* add __init__.py with addon information
* add active and alt_mode key indicators to operator overlays
* add custom HUD UI for all operators and allow viewport navigation event passthrough
* add initial menu
* add initial UI panel
* add new_sketch operator
* add overlay pinning option for all operators
* add spinner operator
* add spinner to UI panel and menu, reorganise operators, update icons
* add thickener modifier
* add view alignment operator, and relatedly fix incorrect overlay redraw implementation — subsequently applied across all other operators
* allow duplicate selection shortcut pass-through in new_sketch operator
* allow mm based factors to be scaled up and down on all operators
* create a dedicated overlay manager, drawing utilities, and update all operators respectively
* ensure cutter bolts are clearly visible in the viewport, including their depth into the target
* step bolt operator segments up by 2, and by 1 on shift, following similar operation to the sketch_bevel operator
* unify input controls across all operators and add revert/cancel functionality


### Bug Fixes

* add poll method to operators to ensure all conditions are correct before they can be invoked
* add shade_smooth call to faux_bevel operator and remove legacy mouse_x/y variables
* add smooth shading step to faux bevel operator
* ensure faux bevel weighted normal weight is set to 100% to avoid face-level artifacts
* ensure new sketches can only be created in object mode with no objects selected
* ensure utils.set_3d_cursor handles the different possible cursor rotation modes
* fix operator labels
* fix register/unregister call for menu in __init__.py
* fix up file names and register all scripts from __init__.py
* set alt mode to constant False on segment property overlay of bolt operator
* set merge_threshold to 0.1mm for screw modifiers on bolt operator
* standardize operator names
* update all operator, panel, and menu class names to follow Blender's naming convention and add execute method to operators for menu support

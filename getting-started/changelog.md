# Changelog

## 1.34.0 (2022-09-19)


### Features

* add a bulk assign ID materials operator (fc3a4c6)
* add a weighted_normal operator along with a new shading category, and move smooth shading into it (8e17737)
* add clean_utils and apply_modifiers ops as shortcuts in main UI panel (7aba702)
* add clear_materials operator (02c580b)
* add CTRL + click modifier removal behaviour to all applicable operators (1fcb674)
* add experimental mode toggle to preferences (4a5a4d1)
* add mirror operation to boolean object fast menu predictions (7df0fea)
* add mouse-step values to lattice, screw, array_cubed, circular_array operators (22e53de)
* add Shift + Alt + E keybinding for the Packaging menu (f92d434)
* add smooth shading and weighted normal operators to the fast-predict menu (28b359a)
* add the id_material operator (20b77a0)
* add undo/redo/W/C event passthrough as experimental feature for geo_lift, panel, and view_align operators (778b064)
* allow bevel segments to be set via mouse movement when mouse values are enabled (c9713bd)
* allow customisation of the overlay base color (b6fb7df)
* allow ID Materials to be actioned in both object and edit mode (face select) (021efe2)
* allow smooth shading operator to be used on multiple objects simultaneously (3d52fc9)
* create a dedicated ID materials menu under Packaging, and a new assign-existing ID material operator (b383f14)
* remove edge weights and vertex groups when clearing edge_bevel, or vertex_bevel operations (bfac62e)
* set keep_sharp for the weighted_normal operator by default (3856be3)
* split applicable util ops into dedicated scene and export menus (6422a49)
* update the ID Materials menu to show a static list of all available colours with previews (bf9d5c1)


### Bug Fixes

* ensure mod order is rectified when using the edge_bevel operator (ecd49d9)
* ensure select objects are made single-user when executing the apply_modifiers operator (a5955fb)
* explicitly import bpy.utils.previews in icons/__init__.py (03f9f2b)
* fix array_cubed manual input override locking (374c00b)
* set profile_extrude's calculate edges option to false by default (d4c7537)

## 1.33.0 (2022-08-06)


### Features

* add clear scale and shrink/fatten to sketch menu for object and edit mode respectively (7be4562)
* add curve support to array_cubed operator (c9b7c88)
* add curve support to screw operator (a74a5e6)
* add curve support to simple_deform operator (bb0fa11)
* add mirror curve option to fast predict menu (6a37a8b)
* add option to mirror curve(s) (def7b2c)
* add screw, array_cubed, and simple_deform curve operators to fast predict menu (0602f21)
* add toggleable exclusive view (x-ray option) option to geo_lift, panel, and view_align operators (9fc75c1)
* split clear_view into overlay (all & custom) options (785fd60)


### Bug Fixes

* ensure make edge/face operation is always available in edit mode fast menu (cbeffac)
* ensure weld modifier removal does not prevent standard bevels from being recalled, and avoid removing HN bevel welds during apply-modifier operations (64c36bd)
* fix lattice target object parenting behaviour (3d8a16e)
* fix the "no predictions found" edge case in the Fast menu with only surfacing recallable operators (b36a447)
* set width lower limit to zero on WN bevel operator (5a5dd78)

## 1.32.0 (2022-06-25)


### Features

* add an option to toggle the sidebar / N-panel (0799e0b)
* add calculate edges option to profile_extrude operator (8d6ead4)
* add extrusion mode option to solidify operator (5011a6f)
* add interpolation mode to lattice operator and default to linear (9fdd252)
* add offset option to profile_extrude operator (e62687c)
* add solidify option to fast menu for non-manifold meshes (a14b819)
* add the ability to recall previous edge bevel weights (e381ab3)
* add toggle wireframe and disable utility modifier options to cycle operator (a3a0bbc)
* enhance profile extrusion and solidification predictions in the Fast menu (539f413)
* ensure mirror modifiers are placed before finishing bevels in the modifier stack (5751adb)
* rectify the mod order for lattice, simple_deform, profile_extrude, screw, solidify, array_cubed, and circular_array operators (2ccb087)
* remove all disabled (viewport hidden) boolean modifiers when using the clean_utils operator (96a82ab)


### Bug Fixes

* add missing fast menu no prediction results section count (ac391ae)
* add missing new_modifier imports to recon_poly, screw_head, set_origin, and triangulate operators (b832ca2)
* ensure single_vertex object has rotation and scale applied after creation (7ce7f30)
* fix edge_bevel width shift/precision and value formatting (78c1cac)
* fix error/crash in clean_utils utility & add logic for lattice modifiers (14cf8a8)
* fix mesh_f2 addon detection in the Fast Predict menu (499d96a)
* fix no predictions logic in the fast menu (1819997)
* fix poll method target object type check in cycle operator (a286253)
* handle object/modifier removal errors more gracefully in clean_utils operator (6da00af)
* unify and lower the merge and bisect thresholds for the mirror operator (843c126)

## 1.31.0 (2022-06-12)


### Features

* add clean geometry logic to view align, and allow view align to be immediately invoked on applicable geometry with an alt mode (db144a6)
* add collapsible sections and common shortcuts to the N panel menu (e57bc0d)
* add inscribed and circumscribed options to recon_poly operator (fa724c4)
* add the panel, geo_lift, and view_align operators to fast menu single object form predictions (94ea2ca)
* automatically collapse new modifiers added to objects (752de82)
* extend inscribed and circumscribed feature to recon_poly inner_radius option & fix recall/revert behaviour (1611885)
* remove problematic bevels from all boolean reference objects (6349c4d)


### Bug Fixes

* ensure viewport camera is always set to orthographic when using view_align operator (ee5c03d)
* fix array_cubed count reset behaviour while respecting the currently specified offset value (a1d5ca5)
* fix direct object view_align operation when utilising edges or vertices (c5059eb)
* fix mirror across geometry behaviour and unneeded show_in_front assignment for evaluated geometry (bd0f14f)
* fix up single and multi-object geometry mirror object evaluation and empty parenting (e7220ad)

## 1.30.0 (2022-06-06)


### Features

* add additional screw head types (@Shaddow) (b130d78)
* add better boolean and sketch detection in the fast prediction menu (3c06550)
* add clean_utils operator (3f4e47b)
* perform additional geometry cleanup when extracting faces using the panel operator (9e53d4b)


### Bug Fixes

* ensure boolean swap_solver updates only apply to objects referencing the selected utils (6845d30)
* ensure clean_utils also handles mirror and array empty objects in utils collection (43c0c82)
* ensure that individual faces cannot be toggled until the inset stage in the panel operator (e6cb10f)
* fix create_duplicate_liftable_geometry object_name parameter being overridden (11d7b4b)
* fix error when using swap solver on a utility referenced by an object with invalid boolean modifiers present (20045ed)
* fix NoneType object error when cycling through a utility object (4a5a402)

## 1.29.0 (2022-06-02)


### Features

* add hard-apply mode to apply_modifiers utility, and exclude regular multi segment edge bevels from normal usage (a5ee288)
* add mirror operator to the fast menu for profile predictions (74f2545)
* add ND theme (color) options to preferences (1d25644)
* add panel operator (a4e76aa)
* add recon poly detection to fast menu (de87d9b)
* add remaining boolean operations to the fast menu (5db12e6)
* add shift alt-mode to set_origin utility to undo faux origin translations (43202bf)
* add solidify and profile extrude options to the fast menu when operators have been previously performed on the selected object (84fa5a0)
* clean up duplicated mesh by default when using geo_lift or panel operators, with option to preserve geometry (d27a8ab)
* detect additional existing mods in fast menu (c0a5963)
* ensure starting geometry is reselected when reverting geo_lift operator (321d2c9)
* harden up circular_array operator, add displacement axis option, and regular/faux origin alt mode (48b5040)


### Bug Fixes

* add an additional clause to the circular_array poll method (11dc8ee)
* add missing continue statements in create_duplicate_liftable_geometry (c6c9aad)
* ensure the inset stage only begins if one or more faces have been selected when using the panel operator (fd26650)
* ensure the reference object origin is restored when cancelling a new circular array operation (00be593)
* fix mod reference error in create_duplicate_liftable_geometry function in object library (979646d)
* fix profile extrude recall and revert behaviour (a9a870d)
* fix recon poly local Z axis natural rotation and recall ability (85e91a1)
* tidy up and fix undesired relative offset behaviour in panel operator (91bbb06)

### 1.28.4 (2022-05-28)


### Bug Fixes

* add additional checks to bevel types in automatic modifier reordering logic (73ce5cf)

### 1.28.3 (2022-05-28)


### Bug Fixes

* fix modifier stack ordering when vertex bevel + weld modifiers are present (4b6a4da)

### 1.28.2 (2022-05-27)

### 1.28.1 (2022-05-27)


### Bug Fixes

* fix unexpected float error in Blender 3.1 and limit the possibility of dividing by zero errors on manual user input (1cdac6c)

## 1.28.0 (2022-05-27)


### Features

* add alt mode to vertex bevel to create a vertex group edge bevel (77cfff4)
* add an option to custom default smoothing angle and update & add it across all relevant operators (ed02679)
* add apply_modifiers utility (1ec0150)
* add cycle operator to fast menu for objects with boolean modifiers present (a71896c)
* add decimate and weld operators under the new simplify menu (1c7b454)
* add edge angle limit option to bevel and weight_normal_bevel operators (c44e0b1)
* add enhanced wireframe mode toggle to all bevel operators (03933cf)
* add fast prediction menu (eb26d59)
* add flip normals option to screw operator (768f1be)
* add natural rotation option to recon poly (980fde9)
* add option to place modifiers at the top/bottom of the stack across edge_bevel, vertex_bevel, and mirror (fc08803)
* add swap_solver utility (5481109)
* add the option to disable automatic update checks in preferences (fbcb91d)
* allow for manual values to be supplied to overlay & optimise operator overlay options (bffaf72)
* allow hydrate utility to be run on multiple selected objects (12fc16e)
* automatically move booleans under WN bevels and single segment HN bevels (1170f08)
* bind the fast menu to F and add a shortcut for Blender's underlying make edge/face operator (b211a23)
* improve the mod ordering logic and apply it to the weld and decimate modifiers (5307ed0)


### Bug Fixes

* add a check to apply_modifiers for disabled modifiers and remove them instead of applying (ffc655a)
* add missing draw_hint import to edge_bevel operator (7aec17d)
* display no prediction message when in edit mode and no precondition matches (7154241)
* fix up has_mod_* logic in fast menu single object predictions (3f27ee3)
* fix weighting calculation in profile_extrude operator (4cd46fb)
* remove triangulate modifier & switch v3_average for .calc_center_median for face points in snap_align operator (0842b3c)

## 1.27.0 (2022-05-14)


### Features

* add Flare (Lighting) operator (83e9be0)
* add option to automatically run solidify after a recon poly operation (9a5dff3)
* add option to capture 2 points in snap_align to align the selected object at the midpoint (21b7a0a)
* add recall ability to circular_array operator (1ff93e8)
* add snap_align operator (7548c66)
* add temporary triangulation to active object during snap_align operations to increase face points (640bc8c)
* allow circular_array operator to be used on a single selected object, and alter origin/translation logic (d273720)
* allow snapping to occur through objects occluding the target while using snap_align (8301845)
* enhance lattice modifier behaviour and allow it to be recalled (10dc6f9)
* hide circular_array empties on completion and give them an appropriate name (c04c466)


### Bug Fixes

* ensure active boolean utils don't affect the geometry of the target object while using snap_align (e796693)
* ensure guideline in snap_align operator is cleared when capture rotation is reset (374ad50)
* ensure mirror selected object show_in_front mode is disabled on complete/cancel (e2d0e07)
* ensure simple deform angle decrements as intended using the step_down key event (9e7b91a)
* ensure snap_align operator supports meshes with vastly different edge lengths (e9de396)
* ensure that the reference object is solo-selected when completing a snap_align operation (73ff168)
* fix circular array revert behaviour for single object mode (f14b5d2)
* fix error when using cycle operator on objects with objectless booleans in their modifier stack (d1bc6cf)
* fix left-click handling for operators that need to pass through the event (8a335b2)
* fix mirror over geometry empty's matrix parent inverse (9a16503)
* fix up circular_array and lattice overlay option control key labels (22e7e54)
* only detect click events on release when using interactive operators (ee19d30)
* remove light energy offset limits (1eb7964)

## 1.26.0 (2022-05-07)


### Features

* add enter & space key presses as additional operator finalisation events (5e3eb6f)
* add modifier & utility cycle operator (73bf7a3)
* add option to mirror across faces, edges, or vertices on selected object (1ebc4ac)
* add shift option to vanilla boolean operator to protect reference object (do not convert into utility) (9efae25)
* add simple_deform operator (d5acf67)
* add triangulate modifier (2e990f8)
* allow for multiple utils to be selected with cycle operator (8bb923b)
* allow mirror modifier to be applied to multiple objects simultaneously (80467d1)
* automatically set geometry mirror axis to Z and flipped (426ed79)
* move sketch operators into their own sub-menu (08bb8fd)
* tidy up main menu by creating Replication and Deformation sub menus to house appropriate operators (6cf9461)


### Bug Fixes

* ensure boolean operators isolate the reference object in the utils collection (14dfdf4)
* ensure mirror empty object is removed if mirror operator is cancelled after geometry selection (9c13ab6)
* fix alt key value change behaviour on cycle operator (9efadc8)
* fix geo_lift operator event handling order (447c654)
* fix recon poly width option overlay display value (8413096)
* fix reference/target object parenting in circular_array operator (7df4058)
* fix up mirror across geometry invalid selection cleanup logic (97873a4)
* update set_lod_suffix mode type in utils_menu (73aa1e7)

## 1.25.0 (2022-04-29)


### Features

* add clear vertex groups utility (ef5e5d5)
* add isolated vertices in selection to active group in vertex bevel recall (b62c55c)
* add recall functionality to vertex bevel operator (7b5cd83)
* add shortcut for isolated utils menu (dcfdf35)


### Bug Fixes

* fix circular array revert behaviour (0d61d74)
* match target object rotation in circular_array operator (7ea17b0)
* remove set rotation from faux set_origin (e371881)
* replace center of volume with bounding box calculation in lattice operator (22add82)

## 1.24.0 (2022-04-26)


### Features

* add alt mode to geo_lift operator to ignore all bevels when calculating selectable geometry (2aff5bc)
* add bool_inset operator (3f29af5)
* add edge_bevel operator (9d876f4)
* add harden normals option to vanilla bevel operator (7827900)
* add lattice operator (fd6eae0)
* add mode option shortcut key for bool_inset operator (5fc4d30)
* add option to lock overlay pin state and position across all operators (0ce0dd7)
* add outset mode to bool_inset operator (cc8edd7)
* add toggle option shortcut keys to applicable operators (c10b066)
* add traditional (now default) and faux origin translation to set_origin utility (5122bae)
* allow for -360 degree rotation on screw operator (306a3e2)
* set face strength mode and face influence on wn_bevel modifiers (eb7cd25)


### Bug Fixes

* add additional checks to all operator poll methods to avoid selection (and order) based errors (cfdde4c)
* ensure circular_array operator allows for traditional (now default) and faux origin translation (a21a46c)
* remove all ND menus from info header bar (db17157)
* set miter_outer to arc in bevel operator (fc4420b)

## 1.23.0 (2022-04-22)


### Features

* allow array_cubed count to roll faux negative (9138c66)
* distinguish between built-in and custom screw head types in the operator overlay, and add additional .blend file cleanup on revert (a37a5bf)

## 1.22.0 (2022-04-22)


### Features

* add array_cubed operator and deprecate square_array (d90dec6)
* add custom screw heads (.blend file) option to addon preferences (539d982)
* add enhanced axis visualization to array_cubed, mirror, profile_extrude, and screw modifiers (9d2cd74)
* add toggle for "fast" booleans in addon preferences and set default to true (previously "exact") (43afa87)
* allow circular_array operator to be run on objects, empties, and at arbitrary rotations (45cb48b)
* show axes on selected object when using the array_cubed operator (77a2a85)


### Bug Fixes

* match target object rotation in set_origin operator (09da9e8)

## 1.21.0 (2022-04-18)


### Features

* add mouse values mode, and integrate all applicable operators (a873f74)
* add profile option to vanilla bevel operator (ca24b38)


### Bug Fixes

* ensure a weld modifier is placed after a vanilla bevel modifier (5cecea6)
* ensure the previous profile value is retained when summoning & reverting a vanilla bevel operator (733f6ad)
* fix profile option behaviour on vertex_bevel operator (9f22e77)
* swap width and segments options on vertex_bevel operator to align with vanilla bevel operator (c9c7e6b)
* update recon_poly option ordering to better align with other operators (width > segments > etc.) (4c107e9)

### 1.20.1 (2022-04-17)


### Bug Fixes

* ensure all scene objects are deselected before executing core single_vertex operator functionality (43b4e6d)

## 1.20.0 (2022-04-17)


### Features

* allow customization of overlay pin and pause keybinds (aae7e91)
* organise addon preferences panel and expose Blender keymap settings (35c26bb)
* split blank_sketch into single_vertex and make_manifold operators (08f6efe)


### Bug Fixes

* fix incorrectly labled profile_extrude overlay alt/ctrl key options (8134622)

## 1.19.0 (2022-04-12)


### Features

* add hydrate operator (a4aef0f)
* add option to enable quick favourites on primary menu (1e8805d)
* add optional late-invocation mode to vertex bevel operator (for post-sketch usage) (ff0ffa4)
* add ortho_grid to toggle_clear_view operator (5e4f8de)
* add viewport menu (with various initial toggles) (1d09367)
* automatically place boolean reference and circular array rotator objects in a utils collection (name configurable in preferences) (eece58b)


### Bug Fixes

* ensure all objects in utils collection are toggled along with the collection consistently (1316fff)
* fix object visibility error in toggle_utils_collection operator (52f3ada)

## 1.18.0 (2022-04-09)


### Features

* add square_array operator and create arrays sub-menu (14ea44e)
* allow active overlay values to be updated with arrow and WASD keys (dbb30c9)


### Bug Fixes

* ensure ND keymap is included in 3D View, Mesh, and Object Mode by default (95498b1)

## 1.17.0 (2022-04-05)


### Features

* add a message/button to the shortcut menu & a link to the changelog in the UI panel when an update is available (bd754cb)
* add bevel operator (126af0d)
* add circular_array operator (8d6d20e)
* adjust circular array option order, add even/odd count step, and allow negative arc angles (b9dedf0)
* ensure mirror modifier bisects selected axis & add flip option for negative axis mirroring (10ddb3d)
* organise operators by relevance in the shortcut menu (b450ba9)
* update documentation section on main UI panel & add Discord link (b5c2d0f)


### Bug Fixes

* ensure operate is only executed on interactive option mutation (8fa29fc)

## 1.16.0 (2022-04-03)


### Features

* add overlay DPI control to preferences (479710b)


### Bug Fixes

* ensure overlay option precision mode indicator is inactive when in pause mode (55ed7ba)
* ensure that the screw operator calculates the order of edges for correct normals (a991db7)

## 1.15.0 (2022-04-02)


### Features

* add manifold option to blank_sketch operator (aebd11b)
* add profile_extrude operator (331f2bb)


### Bug Fixes

* ensure solidify modifier uses even offset (57a5e59)

## 1.14.0 (2022-04-01)


### Features

* add mirror operator (1196540)
* automatically select and set active the boolean reference object (8ea087c)


### Bug Fixes

* ensure that parented objects in all boolean operations have their transforms maintained (82e58a2)

## 1.13.0 (2022-04-01)


### Features

* rename ring_and_bolt to recon_poly (regular convex polygon) as it more accurately represents its behaviour (4837554)

## 1.12.0 (2022-03-31)


### Features

* add boolean slice operator (722dd8d)
* ensure reference and secondary objects in boolean operations are parented to the primary object (7633792)
* prefix boolean reference object names (6044792)

### 1.11.2 (2022-03-30)


### Bug Fixes

* ensure ESC key does not cancel paused operators (01cfa93)

### 1.11.1 (2022-03-30)

## 1.11.0 (2022-03-29)


### Features

* add the 3 core boolean operators, difference, union, and intersect (ca58b0b)


### Bug Fixes

* swap origin and destination objects in set_origin operator (8f84279)

## 1.10.0 (2022-03-27)


### Features

* add version detection, "update available" notification, and Gumroad link to main UI panel (c70b2ff)


### Bug Fixes

* fix erroneous unregister_draw_handler calls in screw, solidify, seams, and smooth operators (02a52d8)

## 1.9.0 (2022-03-27)


### Features

* replace overlay fixed pin location with pin-in-place functionality (2763a33)


### Bug Fixes

* ensure seams operator turns on object auto smooth if override is set (68b58ce)
* fix screw operator summon & revert error (f34b62d)

## 1.8.0 (2022-03-26)


### Features

* add interactive UV seams & sharps operator (a47891a)

### 1.7.1 (2022-02-25)


### Bug Fixes

* ensure the decimate modifier retains its appropriate position in the stack when recalling the ring_and_bolt operator (03117a2)

## 1.7.0 (2022-02-19)


### Features

* add smooth operator (677309e)


### Bug Fixes

* ensure vertex_bevel operator always places current bevel modifier at the top of the stack, and only creates one weld modifier in total (00cfd4e)

### 1.6.1 (2022-02-18)


### Bug Fixes

* reduce remove double vertices threshold in blank_sketch operator (511d311)
* update scale parameter overlay representation in screw_head operator (e153004)

## 1.6.0 (2022-02-08)


### Features

* add 3 point view-plane creation via vertex select mode in view_align operator (3406bd3)
* add profile parameter to vertex bevel (e9ecf35)
* add set_origin utility operator (f271de7)
* add summon behaviour to screw, solidify, and wn_bevel operators (2464274)
* add summon feature to ring_and_bolt operator (b7f1ed7)
* split face_sketch operator into geo_lift and view_align, with improvements in each respectively (9b8d2d4)


### Bug Fixes

* add vert, edge, face specific selection mode to geo_lift operator (9e91e06)
* ensure all target geometry is deselected when first entering geo_lift, or view_align operators (83bc45d)
* ensure cancel keybind cancels all operators, particularily while in halt mode (126ec13)
* ensure correct leftover geometry is removed based on selection mode in geo_lift operator (0ea0be0)
* ensure summoned ring_and_bolt operator reverts back to previous values on cancel (4dbc91c)
* fix solidify operator weighting label array index error (f3eabc8)
* remove unneeded viewport cursor wrap behaviour (26a14c6)

## 1.5.0 (2022-02-06)


### Features

* add screw head generator (c91ac08)
* add toggleable "halt" mode to all operators, allowing event / keybinding passthrough (1ec0942)


### Bug Fixes

* add planar decimate modifier to ring_and_bolt objects if the segment count is greater than 3 (d92dc02)

## 1.4.0 (2022-02-04)


### Features

* add utils menu as sub-menu on main menu (2d88ed2)

## 1.3.0 (2022-01-31)


### Features

* add a dynamic relationship between inner radius and width parameters, for more predictive results, and better ring generation (03b15f6)


### Bug Fixes

* enforce 0.0001 minimum width for weighted normal bevel, and add WN prefix to bevel modifier name for better recognition (2831254)

### 1.2.1 (2022-01-30)


### Bug Fixes

* fix broken keymap entry property name for main menu after name change (3cf72cb)
* use more reliable collection objects link call for operators creating single vertex objects (58d433a)

## 1.2.0 (2022-01-30)


### Features

* add name_sync operator and new ND Utils UI panel (dfcc13d)
* add set_lod_suffix operator (3e9cdb1)
* allow F key passthrough on face_sketch operator (a8e4e3a)


### Bug Fixes

* clear custom split normals on extracted faces in face_sketch operator (f33ac67)
* ensure clean up method in face_sketch operator removes extracted face when the operation is cancelled (17cb5e1)
* fix incorrect class name unregister call in main_menu.py (b11a97b)
* fix poll method qualifier in name_sync operator (8c5f585)
* set the bevel modifier offset type to 'width' for the vertex_bevel, and weighted_normal_bevel operators (9b561aa)

### 1.1.1 (2022-01-29)


### Bug Fixes

* add missing capture_modifier_keys function call to invoke method on face_sketch operator (573d0d2)
* remove hardcoded mm suffix on all operator overlay parameter labels (c5a253e)
* set starting width parameter to 0 on vertex_bevel operator (130f8ef)

## 1.1.0 (2022-01-29)


### Features

* add face extraction mode to view_align operator and rename it to face_sketch, rename new_sketch to blank_sketch, and sketch_bevel to vertex_bevel (2a04917)
* rename operators - spinner to screw, thickener to solidfiy, and faux_bevel to weighted_normal_bevel (c7e4d2c)
* split offset and thickness modifiers from bolt operator in favour of solidy operator usage, add ring functionality to bolt operator, rename bolt to ring_and_bolt (4585823)


### Bug Fixes

* add invalid face selection error handling for face_sketch operator (32a491a)
* ensure update_overlay function is called after every event type (c5d59b0)
* fix ring_and_bolt parameters and parameter names to more appropriately represent their behaviour (6ee7a6b)
* update solidify weighting parameter name (5586b69)

## 1.0.0 (2022-01-28)


### Features

* add __init__.py with addon information (77a92de)
* add active and alt_mode key indicators to operator overlays (bde234c)
* add custom HUD UI for all operators and allow viewport navigation event passthrough (e032770)
* add initial menu (a6329b3)
* add initial UI panel (789f471)
* add new_sketch operator (3aca34b)
* add overlay pinning option for all operators (8bff7c4)
* add spinner operator (26c1aea)
* add spinner to UI panel and menu, reorganise operators, update icons (bbc1002)
* add thickener modifier (f215357)
* add view alignment operator, and relatedly fix incorrect overlay redraw implementation — subsequently applied across all other operators (7eabac6)
* allow duplicate selection shortcut pass-through in new_sketch operator (86255a0)
* allow mm based factors to be scaled up and down on all operators (c433400)
* create a dedicated overlay manager, drawing utilities, and update all operators respectively (1520b36)
* ensure cutter bolts are clearly visible in the viewport, including their depth into the target (d6d08f2)
* step bolt operator segments up by 2, and by 1 on shift, following similar operation to the sketch_bevel operator (8dbece2)
* unify input controls across all operators and add revert/cancel functionality (5a79040)


### Bug Fixes

* add poll method to operators to ensure all conditions are correct before they can be invoked (4faad28)
* add shade_smooth call to faux_bevel operator and remove legacy mouse_x/y variables (0d994b7)
* add smooth shading step to faux bevel operator (5f09d2c)
* ensure faux bevel weighted normal weight is set to 100% to avoid face-level artifacts (0849dfd)
* ensure new sketches can only be created in object mode with no objects selected (d77f839)
* ensure utils.set_3d_cursor handles the different possible cursor rotation modes (b7100ec)
* fix operator labels (18023dc)
* fix register/unregister call for menu in __init__.py (7683f8d)
* fix up file names and register all scripts from __init__.py (94dd2b9)
* set alt mode to constant False on segment property overlay of bolt operator (99e4a12)
* set merge_threshold to 0.1mm for screw modifiers on bolt operator (5d0c064)
* standardize operator names (c25991e)
* update all operator, panel, and menu class names to follow Blender's naming convention and add execute method to operators for menu support (86c96dd)

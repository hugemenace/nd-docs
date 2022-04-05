# Changelog

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

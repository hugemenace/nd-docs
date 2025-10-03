# View Align

The View Align operator will create a virtual copy of the selected object with modifiers applied, allowing you to select geometry to focus the viewport camera on & look directly at. This operation will also place the 3D at the center of the selected geometry, create a custom transform orientation, and rotate the 3D cursor to align with the selected geometry's normal.

## Options

| Option | Shortcut | Mouse Value Compatible | Description |
| :--- | :--- | :--- | :--- |
| Selection Type | **`S,1,2,3`** | No | The geometry selection type (Vertex, Edge, or Face) |
| Exclusive View | **`E`** | No | Show the target object in front of all other objects |

## Alternative modes

Hold down the shortcut when selecting the operator to enter the respective mode.

| Shortcut | Description |
| :--- | :--- |
| **`SHIFT`** | Do not clean duplicate mesh before extraction |
| **`ALT`** | Skip geometry selection and use the active object |

---

?> With [experimental mode](/getting-started/preferences) enabled, you'll be able to use `ctrl + z` (undo), `shift + ctrl + z` (redo), `W`, and `C` (selection) hotkeys.
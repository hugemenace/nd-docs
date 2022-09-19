# Panel

The Panel operator combines several actions: Geo Lift, Inset, and Solidify. Useful when creating panels, as the name suggests, or extracting geometry for boolean operations.

[](../_media/panel.mp4 ':include')

## Alternative modes

Hold down the shortcut when selecting the operator to enter the respective mode.

| Shortcut | Description |
| :--- | :--- |
| **`SHIFT`** | Do not clean duplicate mesh before extraction |

## Options

### Step 1 (Select)
| Option | Shortcut | Mouse Value Compatible | Description |
| :--- | :--- | :--- | :--- |
| Confirm Geometry | **`SPACE`** | No | After selecting the faces to extract, hit the space bar to continue |
| Exclusive View | **`E`** | No | Show the target object in front of all other objects |

### Step 2 (Inset)
| Option | Shortcut | Mouse Value Compatible | Description |
| :--- | :--- | :--- | :--- |
| Inset Amount | _None_ | **Yes** | The amount to inset the selected faces |
| Individual Faces | **`F`** | No | Whether to inset the faces individually, or as a unified group |
| Exclusive View | **`E`** | No | Show the target object in front of all other objects |

### Step 3 (Solidify)
Same options as those present in the [Solidify](/extrusion/solidify) operator.

---

?> With [experimental mode](/getting-started/preferences) enabled, you'll be able to use `ctrl + z` (undo), `shift + ctrl + z` (redo), `W`, and `C` (selection) hotkeys.
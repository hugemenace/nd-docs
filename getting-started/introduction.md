# Introduction to ND

ND (short for non-destructive) is a Blender addon that provides a number of workflow enhancements, tools, operations, and generators — tailored specifically for non-destructive modelling. 

This approach is useful for many types of modelling needs, particularly hard-surface forms, while being able to quickly adjust parameters without the need for manual poly-modelling. ND makes extensive use of modifiers to enable this flexible workflow.

## How to open it

ND can be accessed in 2 distinct ways, via the N panel, located under the "HugeMenace" tab — or via the shortcut menu bound to **SHIFT + 2** (you can change this under _Edit > Preferences > Keymap_).

## How to use it

The ND addon works in different Blender modes (object & edit) and changes behaviour depending on how many objects you have selected. At any point, you can open the N panel UI or the menu and see which operators are available given your current context (operators which cannot be used will be disabled automatically).

For operators that work interactively, an overlay will appear next to and follow the mouse cursor. If you would like to **pin** the overlay in place, you can hit **P** key. Each press will toggle pinning on/off. 

Overlay's have a special **Pause** mode which can be toggled by hitting the backslash key **\**. This will pause the operator and allow you to perform other actions in Blender.

Certain operators (those with [R] next to their name in the docs) can be **Recalled**. When an operator is recalled, the current modifier settings used by the object be automatically loaded into the overlay, so you can continue where you left off or adjust the previous operation.

In some situations the overlay can be in multiple states, for example, both pinned & paused.

### Overlay states

| Overlay State | Description |
| :------------ | :----------- |
| ![Overlay](../_media/overlay.jpg) | The standard overlay state. |
| ![Overlay Pinned](../_media/overlay-pinned.jpg) | The pinned overlay state. |
| ![Overlay Paused](../_media/overlay-paused.jpg) | The paused overlay state. |
| ![Overlay Paused Pinned](../_media/overlay-paused-pinned.jpg) | The paused & pinned overlay state. |
| ![Overlay Recalled](../_media/overlay-recall.jpg) | The recalled overlay state. |

## Operator options

Most operators while in an interactive mode will have one or more options. These are shown in the overlay prefixed with a grey dot. The current active option is always prefixed with a blue dot.

When pressing and holding the modifier key shown under any option, the option will be activated and the blue dot will be shown next to it. When the modifier key is released, the option will be deactivated and the blue dot will be hidden.

?> **Important:** To change an option's current value, simply use your **mouse scroll wheel** (scroll up to increase and down to decrease).

Many operator options have a _precision_ mode which can be activated by holding down the **SHIFT** key. You'll know when an active option is in this mode as the option's blue dot will be half-filled.

?> For certain options, the step size can be altered by hitting the plus and minus keys on the numpad or the keyboard.

| Overlay Option | Description |
| :------------ | :----------- |
| ![Overlay Option](../_media/overlay-option.jpg) | An overlay with multiple options. The active option is shown by a blue dot. |
| ![Overlay Option Precision](../_media/overlay-option-precision-mode.jpg) | An overlay with the active option in _precision_ mode. |

## Adjusting the overlay

If the overlay text is to small to read on your monitor (for instance you're using a 4K resolution) - you can increase the size by adjusting the _Overlay DPI_ in the addon preferences.

![Overlay DPI](../_media/overlay-dpi-out.jpg)
# Introduction to ND

ND (short for non-destructive) is a Blender addon that provides a number of workflow enhancements, tools, operations, and generators — tailored specifically for non-destructive modelling. 

This approach is useful for many types of modelling needs, particularly hard-surface forms, while being able to quickly adjust parameters without the need for manual poly-modelling. ND modelling makes extensive use of modifiers to enable this flexible workflow.

## How to open it

ND can be accessed in 2 ways, via the 3D scene view N panel, located under the "HugeMenace" tab, or via the shortcut menu bound to **SHIFT + 2** (you can override / change the key binding in your Blender settings).

## How to use it

The ND addon works in various different modes (object & edit), and in relation to how many objects, or the lack thereof, are selected. At any point, you can open the N panel UI or the menu, and see which operators are available given the current scene context (operators which cannot be used will be disabled automatically).

For operators that work interactively, a floating UI will appear next to and follow the mouse cursor. If you would like to **pin** the overlay in place, you can hit **P** key. Each press will toggle pinning on/off. 

ND's operators and floating UI have a special **Pause** mode which can be enabled by hitting the backslash key **\**. This will pause the operator and allow you to perform other operations in Blender, before unpausing ND and continuing with the operation.

Certain operators (those with [R] next to their name in the docs) can be **Recalled**. When an operator is recalled, the previous settings used by the operator on the selected object will be automatically re-loaded, so you can continue where you left off, or allow you to tweak the previous operation.

In some situations the overlay can/may be in multiple states, eg.: both pinned & paused.

### Overlay states

| Overlay State | Description |
| :------------ | :----------- |
| ![Overlay](../_media/overlay.jpg) | The standard overlay state. |
| ![Overlay Pinned](../_media/overlay-pinned.jpg) | The pinned overlay state. |
| ![Overlay Paused](../_media/overlay-paused.jpg) | The paused overlay state. |
| ![Overlay Paused Pinned](../_media/overlay-paused-pinned.jpg) | The paused & pinned overlay state. |
| ![Overlay Recalled](../_media/overlay-recall.jpg) | The recalled overlay state. |

## Operator options

Most operators while in an interactive mode will have one or more options. These are shown in the overlay prefixed with a grey dot, while the active option is prefixed with a blue dot.

When pressing the modifier key as shown next to each option, the option will be activated, and the blue dot will be shown next to the option to let you know any changes will be applied to that option.

?> **Important:** To change an options value, you use your **mouse scroll wheel** (up to increase, down to decrease).

Many operator options have a "precision" mode which can be activated by holding down the **SHIFT** key. You'll know when an active option is in this mode, as the option will be prefixed with a half-filled blue dot.

?> For certain options, the step size can be altered by hitting the plus/minus keys on the numpad.

| Overlay Option | Description |
| :------------ | :----------- |
| ![Overlay Option](../_media/overlay-option.jpg) | An overlay with multiple options, with the active option shown by a blue dot. |
| ![Overlay Option Precision](../_media/overlay-option-precision-mode.jpg) | An overlay with the active option in precision mode. |

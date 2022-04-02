# Set Origin

The Set Origin operator will translate the reference object to the origin of the target object, and then use displacement modifiers to "virtually" translate the reference object back to its original position. This is extremely useful when trying to perform circular arrays on non-destructive objects (eg. Recon Poly) which rely on precise origin placement.

!> In order to make use of this operator, first select the target object and then the reference object's origin you'd like to mimic.

![Set Origin Operator](../_media/set-origin-out.jpg ':size=800')

!> **Note:** This operation should be thought of as a "virtual translation". For cases where you're not dealing with a non-destructive object, Blender's built-in origin management functionality is preferred.
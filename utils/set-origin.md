# Set Origin

The Set Origin operator will translate the reference object to the origin of the target object, and then use displacement modifiers to "virtually" translate the reference object back to it's original position. This is extremely useful when trying to perform circular arrays on non-destructive objects without having to worry about the objects modifiers being screwed up in the process.

!> In order to make use of this operator, first select the reference object and then the target object. The reference object will be the object that is translated.

![Set Origin Operator](../_media/set-origin-out.jpg ':size=800')

!> **Note:** The Set Origin operation should be thought of more as a "virtual translation" operation. For cases where you're not dealing with a non-destructive reference object, Blenders default origin management functionality is preferred.
# Circular Array

The Circular Array operator allows you to array an object around a specific point / object in a cicular or arc-like fashion.

?> **Note:** there are 2 types of behaviour that this operator exhibits: *Circle* and *Arc* mode. Circle mode is is only enabled when the **Angle** is set to exactly **+/-360 degrees**. While in circle mode, each item in the array is spaced evenly around the full circumference of the circle. However, in arc mode the first and last items will sit at the beginning and end of the arc respectively, with the remaining items spaced evenly around the rest of the arc.

![Circular Array Operator](../_media/circular-array-out.jpg ':size=800')

!> **Important:** the object you want to array will need its origin set to the exact same location as the reference object you're rotating around in order to avoid strange behaviour. In cases where you're utilising non-destructive / generative geometry which relies specifically on the origin of the object (eg. Recon Poly), you can use the special [Set Origin](/utils/set-origin.md) operator to set the origin of the object to the same location as the reference object without destroying the generated geometry.

## Options

| Option | Description |
| :------ | :----------- |
| Count | The number of copies to create (minimum value is 2). |
| Axis | The local axis of the target object to rotate around. |
| Angle | The angle of the arc used for the cicular path. |

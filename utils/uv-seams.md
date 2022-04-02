# UV Seams

The UV Seams operator will allow you to interactively set the UV seams for an object based on a specified edge selection angle.

![UV Seams Operator](../_media/uv-seams-out.jpg ':size=800')

!> **Note:** this operator should only be used on objects which have had their modifiers collapsed and may have poor performance on objects with many edges. Future versions of this operator will address these issues.

| Option | Description |
| :------ | :----------- |
| Angle | The minimum angle at which seams will be automatically added to edges. |
| Sync Auto Smooth | Whether or not to update the object's current auto smooth angle to match the selected seam angle. |
# UV Seams

The UV Seams operator will allow you to interactively set the UV seams for the active object based on a minimum specified angle.

![UV Seams Operator](../_media/uv-seams-out.jpg ':size=800')

!> **Note:** this operator should only be used on objects which have had their modifiers collapsed (destructive) and may have poor performance on large complicated objects with many edges. Future versions of this operator will address these issues.

| Option | Description |
| :------ | :----------- |
| Angle | The minimum angle at which seams will be automatically added to edges. |
| Sync Auto Smooth | Whether to update the objects current auto smooth angle to match the selected seam angle. |
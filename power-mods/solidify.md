# Solidify [R]

The Solidify operator will allow you to create a thickened version of a mesh. It's mostly commonly used on planar meshes, turning a 2D silhouette into a 3D object.

![Solidify Operator](../_media/solidify-out.jpg ':size=800')

## Options

| Option | Description |
| :------ | :----------- |
| Thickness | The thickness of the solidification. |
| Weighting | There are 3 weight options: *Positive*, *Negative*, and *Neutral*. Positive and negative will locate the solidified output inside or outside the original mesh determined by the face normals. With Neutral, the solidified output will be centered on the original mesh. |
| Offset | The amount of optional offset to apply after solidification (useful when creating boolean reference objects.) |

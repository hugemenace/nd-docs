# Solidify [R]

The Solidify operator will allow you to create a solidified (thickened) version of an object. It's best utilised on sketches, allowing you to create a solidified version of a sketch without destroying the original sketch.

![Solidify Operator](../_media/solidify-out.jpg ':size=800')

## Options

| Option | Description |
| :------ | :----------- |
| Thickness | The thickness of the solidification. |
| Weighting | There are 3 weighting options, *Positive*, *Negative*, and *Neutral*. Positive and negative will locate the solidified output inside or outside the original mesh determined by the face normals. With Neutral, the solidified output will be centered on the original mesh. |
| Offset | The amount of optional offset to apply after solidification (useful when creating cutter objects for boolean operations which need to protrude from the target object in order to work correctly). |

# Profile Extrude [R]

The Profile Extrude operator will allow you to extrude a 2D (edge-based) profile. It's best utilised on non-manifold sketches as a precursor to running the solidify operator.

![Profile Extrude Operator](../_media/profile-extrude-out.jpg ':size=800')

## Options

| Option | Description |
| :------ | :----------- |
| Extrusion | The length of the extrusion. |
| Weighting | There are 3 weighting options, *Positive*, *Negative*, and *Neutral*. Positive and negative will extrude inside or outside the original mesh determined by the face normals. With Neutral, the extrusion will be centered on the original mesh. |
| Axis | The axis to extrude along. |

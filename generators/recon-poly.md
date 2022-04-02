# Recon Poly [R]

The Recon Poly generator allows you to quickly and easily generate any regular convex polygon (triangles, squares, hexagons, etc.) with an optional hole in the center.

![Recon Poly Generator](../_media/recon-poly-out.jpg ':size=800')

?> **Note:** this operator is "smart" in the sense that it will automatically swich between `width` and `radius` depending on whether you have an `inner radius` set and automatically limit the value to avoid overlapping geometry.

## Options

| Option | Description |
| :------ | :----------- |
| Segments | The number of sides. |
| Inner Radius | The radius of the hole in the center. |
| Width / Radius | The width of outer visible area (when used alongside an inner radius) or the radius of the overall polygon. |

# Ring and Bolt [R]

The ring and bolt operator allows you to quickly and easily generate any regular convex polygon (triangles, squares, hexagons, etc.) with an optional additional hole in the center.

![Ring and Bolt Generator](../_media/ring-and-bolt-out.jpg ':size=800')

?> **Note:** this operator is "smart" in the sense that it will automatically swich between `width` and `radius` depending on whether you have an `inner radius` set or not, and automatically adjust the value within sensible limits. This will ensure you don't end with strange overlapping geometry.

## Options

| Option | Description |
| :------ | :----------- |
| Segments | The number of sides. |
| Inner Radius | (Optional) The radius of the hole in the center. |
| Width / Radius | The width of the ring (when used alongside an inner radius) or the radius. |

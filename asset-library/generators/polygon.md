# Polygon

Generates a polygon with adjustable radius and number of sides. By modifying its parameters, you can create any regular convex polygon, such as a triangle, square, hexagon, or a near‑circular shape.

!> **Note:** this generator requires host geometry to function, please see the [generators overview](/asset-library/generators/overview).

## Standard Parameters

| Parameter | Description |
| :--- | :--- |
| `Sides` | Number of sides or “steps” used to generate the shape. Higher values create a form that more closely approximates a circle. |
| `Radius` | Radius of the polygon. The meaning of this value depends on whether the polygon is _Inscribed_ or circumscribed. |
| `Start Angle` | Starting angle of the generated geometry. For example, a polygon with 3 sides and a start angle of 0° forms a triangle pointing to the right when viewed from above, while a start angle of 90° points it upwards. |
| `Inscribed` | Determines whether the vertices of the polygon sit within the given radius, as opposed to the edges forming tangents to the implicit circular shape defined by the radius. |

## Advanced Parameters

| Parameter | Description |
| :--- | :--- |
| `Material` | ➥ See [common parameters](/asset-library/common-parameters). |
| `Next Reference` | ➥ See [common parameters](/asset-library/common-parameters). |

## Metadata

| Icon |
| --- |
| ![ND.Polygon](../../_media/asset-library/ND.Polygon.png ':size=128') |
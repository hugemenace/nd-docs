# Disc

Generates a disc with adjustable inner radius and width. By modifying its parameters, you can also create other polygonal shapes, not just discs.

!> **Note:** this generator requires host geometry to function, please see the [generators overview](/asset-library/generators/overview).

## Standard Parameters

| Parameter | Description |
| :--- | :--- |
| `Width` | "Thickness" of the disc. |
| `Sides` | Number of sides or “steps” generated from the starting position to the end (as defined by the angle). When the angle is 360°, this value determines the number of sides of the resulting regular polygon border. Higher values produce a shape that more closely approximates a circle. |
| `Radius` | Radius of the disc. Whether this is an outer, inner, or midway point radius depends on the selected _Direction_. |
| `Steps` | Number of steps (or cuts) created along the length of the disc. |
| `Direction` | Direction of generated geometry. **Positive** generates geometry extending outward from the radius. **Neutral** generates geometry extending equally outward and inward from the radius. For example, if the width is 100 mm, then 50 mm extends outward and 50 mm inward. **Negative** generates geometry extending inward from the radius. |
| `Flip Normals` | ➥ See [common parameters](/asset-library/common-parameters). |

?> **Hint:** adjusting the number of `sides` lets you create more than just circular shapes. For example, 3 sides produce a triangle, 4 sides a square, and so on. Increasing the number of sides makes the shape progressively closer to a perfect circle.

## Advanced Parameters

| Parameter | Description |
| :--- | :--- |
| `Angle` | Total angle of revolution. For example, a 360° angle would create a circular shape, while a 180° angle would create an arch. |
| `Revolve Axis` | Local axis to revolve around. |
| `Base Axis` | Local axis along which to generate the starting edge before then revolving it around the _Revolve Axis_. |
| `Merge Distance` | ➥ See [common parameters](/asset-library/common-parameters). |
| `Material` | ➥ See [common parameters](/asset-library/common-parameters). |
| `Next Reference` | ➥ See [common parameters](/asset-library/common-parameters). |

## Metadata

| Icon |
| --- |
| ![ND.Disc](../../_media/asset-library/ND.Disc.png ':size=128') |
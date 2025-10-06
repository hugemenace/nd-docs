# Revolve

Revolves the input geometry around a specified axis to generate a lathed surface.

## Standard Parameters

| Parameter | Description |
| :--- | :--- |
| `Revolve Axis` | Local axis around which the geometry is revolved. |  
| `Angle` | Total angle of revolution. A value of 360° produces a closed rotational surface, while smaller values generate partial arcs. |  
| `Segments` | Number of segments (or “steps”) used to interpolate the surface along the revolution. Higher values result in smoother geometry. |  
| `Offset Axis` | Secondary local axis along which the profile is offset before the revolution occurs. |  
| `Offset Amount` | Distance to move the geometry along the offset axis prior to revolving. |  
| `Offset Rotation` | Rotational adjustment applied to the revolved geometry around the defined revolve axis. |  
| `Generate Caps` | Determines whether end caps are created when the revolution does not complete a full 360°. |  
| `Flip Normals` | ➥ See [common parameters](/asset-library/common-parameters). |  

## Advanced Parameters

| Parameter | Description |
| :--- | :--- |
| `Extrude Individual Faces` | Revolves each face independently instead of treating the geometry as a single continuous profile. |  
| `Merge Distance` | ➥ See [common parameters](/asset-library/common-parameters). |  
| `Material` | ➥ See [common parameters](/asset-library/common-parameters). |
| `Context` | ➥ See [common parameters](/asset-library/common-parameters). |  
| `Next Reference` | ➥ See [common parameters](/asset-library/common-parameters). |

## Metadata

| Icon |
| --- |
| ![ND.Revolve](../../_media/asset-library/ND.Revolve.png ':size=128') |
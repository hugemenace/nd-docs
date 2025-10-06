# Array (Circular)

Distributes the geometry around its origin in a circular pattern, or optionally around another target object in the scene.

## Standard Parameters

| Parameter | Description |
| :--- | :--- |
| `Revolve Axis` | Local axis used as the centre of rotation. |  
| `Angle` | Total angle of the circular path along which the array is distributed. A value of 360° creates a complete circle, while lower values, such as 180°, form an arc. |  
| `Count` | Number of copies to generate along the circular path. |  
| `Offset Mode` | Determines how the offset is calculated; either relative to the geometry’s **Origin** or based on another **Object** in the scene. |  

### Offset Mode (Origin) Parameters

| Parameter | Description |
| :--- | :--- |
| `Offset Axis` | Local axis along which the geometry is translated before being arrayed. |  
| `Offset Amount` | Distance the geometry is moved along the offset axis. |  
| `Offset Rotation` | Rotation applied to each arrayed instance around the centre of the circular path. |  

### Offset Mode (Object) Parameters

| Parameter | Description |
| :--- | :--- |
| `Offset Object` | Object used as the centre of rotation for the array. |

## Advanced Parameters

| Parameter | Description |
| :--- | :--- |
| `Context` | ➥ See [common parameters](/asset-library/common-parameters). |
| `Next Reference` | ➥ See [common parameters](/asset-library/common-parameters). |

## Metadata

| Icon |
| --- |
| ![ND.CircularArray](../../_media/asset-library/ND.CircularArray.png ':size=128') |
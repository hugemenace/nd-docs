# Endpoints

Detects mesh endpoints and records their direction and rotation for use in subsequent operations.

## Standard Parameters

| Parameter | Description |
| :--- | :--- |
| `End Attribute` | Boolean attribute name stored in the geometry stream (true for detected endpoints, false otherwise). |
| `Direction Attribute` | Vector3 attribute name stored in the geometry stream (represents the direction of each endpoint, visualised as an arrow extending from its tip). |
| `Rotation Attribute` | Rotation (quaternion) attribute name stored in the geometry stream (captures the final rotation of each endpoint based on the underlying curve’s TBN matrix). |
| `Flip Direction` | Flip the stored direction. |


## Advanced Parameters

| Parameter | Description |
| :--- | :--- |
| `Context` | ➥ See [common parameters](/asset-library/common-parameters). |

## Metadata

| Icon |
| --- |
| ![ND.SelectEndpoints](../../_media/asset-library/ND.SelectEndpoints.png ':size=128') |
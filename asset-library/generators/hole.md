# Hole

Generates a hole cutter with customisable countersink, counterbore, and drill point parameters.

!> **Note:** this generator requires host geometry to function, please see the [generators overview](/asset-library/generators/overview).

## Standard Parameters

| Parameter | Description |
| :--- | :--- |
| `Hole Type` | Switch between **Simple**, **Counterbore**, and **Countersink**. |
| `Drill Point` | Enables a drill‑style angled endpoint representing the material removed by the drill bit. |
| `Segments` | Number of segments (or “steps”) used to create geometry during the revolution process. |
| `Hole Depth` | Depth of the hole. |
| `Hole Diameter` | Diameter of the hole. |
| `Counter Diameter` | Diameter of the counter area (countersink or counterbore) above the main hole. |
| `Counterbore Depth` | Depth of the counterbored area. |

## Advanced Parameters

| Parameter | Description |
| :--- | :--- |
| `Countersink Angle` | Angle of the countersink, measured from the hole's axis (default: 45°). |
| `Drill Point Angle` | Angle of the drill point. |
| `Protrusion Distance` | Specifies how far the protrusion geometry extends above the hole. This stabilises boolean operations in Blender, often reducing the need for the Exact solver. |
| `Merge Distance` | ➥ See [common parameters](/asset-library/common-parameters). |

## Metadata

| Icon |
| --- |
| ![ND.Hole](../../_media/asset-library/ND.Hole.png ':size=128') |
# Path Smooth

Smooths the selected path by bevelling existing corners or resampling the entire curve.

## Standard Parameters

| Parameter | Description |
| :--- | :--- |
| `Corner Segments` | Number of bevel segments; a value of 1 produces a chamfer, while higher values create a rounded fillet. |  
| `Corner Radius` | Radius of the bevel applied to each corner. |  

## Advanced Parameters

| Parameter | Description |
| :--- | :--- |
| `Resample` | Determines whether to resample the smoothed path to achieve evenly distributed curve points. |  
| `Resample Count` | Total number of points to generate when resampling. |  
| `Corner Segment Factor` | Scales the number of corner segments by a factor. For example, if `Corner Segments` is set to 10 and this value is 0.5, the final segment count will be 5. |  
| `Corner Radius Factor` | Scales the corner radius by a factor, behaving similarly to the corner segment factor. |  
| `Merge Distance` | ➥ See [common parameters](/asset-library/common-parameters). |  
| `Context` | ➥ See [common parameters](/asset-library/common-parameters). |  
| `Next Reference` | ➥ See [common parameters](/asset-library/common-parameters). |

## Metadata

| Icon |
| --- |
| ![ND.SmoothPath](../../_media/asset-library/ND.SmoothPath.png ':size=128') |
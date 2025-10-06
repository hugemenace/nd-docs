# Distribute

Distributes referenced geometry across points in the input geometry stream, with flexible control over spawning conditions, randomisation, rotation, and scale.

## Standard Parameters

| Parameter | Description |
| :--- | :--- |
| `Object` | Object to instance on each point that meets the spawn condition. |  
| `Spawn Condition` | Determines how instances are spawned; **Always**, **Boolean**, **Threshold**, or **Weighted Random**. |  
| `Rotation Factor` | hint: factor 0-1. |  
| `Scale Factor` | hint: factor 0-1. |

### Spawn Condition (Boolean) Parameters

| Parameter | Description |
| :--- | :--- |
| `Spawn` | Boolean attribute that determines whether an instance is created at each point. | 

### Spawn Condition (Threshold) Parameters

| Parameter | Description |
| :--- | :--- |
| `Weighting` | Normalised factor (0–1) representing the input weighting used for threshold comparison. | 

### Spawn Condition (Weighted Random) Parameters

| Parameter | Description |
| :--- | :--- |
| `Weighting` | hint: factor 0-1. | 

## Advanced Parameters

| Parameter | Description |
| :--- | :--- |
| `Rotation Axis` | aaaa. |  
| `Rotation Min` | aaaa. |  
| `Rotation Max` | aaaa. |  
| `Scale Min` | aaaa. |  
| `Scale Max` | aaaa. |  
| `Context` | ➥ See [common parameters](/asset-library/common-parameters). |  
| `Preserve Context Geometry` | ➥ See [common parameters](/asset-library/common-parameters). |
| `Next Reference` | ➥ See [common parameters](/asset-library/common-parameters). |

### Spawn Condition (Threshold) Parameters

| Parameter | Description |
| :--- | :--- |
| `Spawn Threshold` | Normalised threshold value (0–1) that determines whether a point spawns an instance based on its weighting. | 

### Spawn Condition (Weighted Random) Parameters

| Parameter | Description |
| :--- | :--- |
| `Random Seed` | Seed value used to introduce controlled variation in weighted random spawning. | 

## Metadata

| Icon |
| --- |
| ![ND.Distribute](../../_media/asset-library/ND.Distribute.png ':size=128') |
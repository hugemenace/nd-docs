# Selectors

Selectors add attributes to the incoming geometry stream (context), enabling other operators such as [Attach](/asset-library/operators/attach) or [Distribute](/asset-library/operators/distribute) to work more intelligently by acting on per‑point data rather than applying the same rules uniformly across all points.

?> **Note:** All selector attribute names are automatically prefixed with `ND.`. For example, when using the [Endpoint](/asset-library/selectors/endpoints.md) selector and a direction attribute named `EndpointDirection`, the final attribute will be stored on the geometry as `ND.EndpointDirection`.
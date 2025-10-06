# Generators

Generators create new base geometry intended to be chained with other modifiers, as opposed to [Operators](/asset-library/operators/overview) or [Selectors](/asset-library/selectors/overview), which operate on existing geometry.

?> **Note:** for a generator to function, it must be placed on _host_ geometry. The host can be any mesh object, as it will be deleted by the generator. For convenience, it’s best to use a single vertex as the host. This requirement exists because Blender does not support placing a Geometry Nodes modifier or network directly into the scene as a standalone entity.

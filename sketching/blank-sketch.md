# Blank Sketch (Deprecated)

!> **Deprecated**: This operator has been split into two new operators, [Single Vertex](/sketching/single-vertex) and [Make Manifold](/sketching/make-manifold). Blank Sketch will eventually be completely removed from the addon. If you would like to utilise it for the short term, it can be re-enabled in the latest release by turning on "Compatibility Mode" in the addon preferences.

The Blank Sketch operator allows you to quickly start with a single vertex and perform a number of extrusions on it to define your 2D shape. When the `manifold` option is enabled (it's on by default), the resulting geometry will have all overlapping vertices removed and edges/faces filled in.

![Blank Sketch Operator](../_media/blank-sketch-out.jpg ':size=800')

?> **Tip:** this operator is a good candidate for using the pause & pin overlay functionality — giving you the freedom to extrude and manipulate the vertices without the operator getting in the way.

## Options

| Option | Description |
| :------ | :----------- |
| Manifold | Ensure the final mesh is manifold. |
# Blank Sketch

The Blank Sketch operator allows you to quickly start with a single vertex and perform a number of extrusions on it to define your 2D shape. When committing the sketch, the resulting geometry will have all closely overlapping (double, triple, etc.) vertices removed and edges/faces filled in if `manifold` is enabled. 

![Blank Sketch Operator](../_media/blank-sketch-out.jpg ':size=800')

?> **Tip:** this operator is a good candidate for using the pause functionality of ND while sketching. Once committed, you can use the solidify operator to convert the sketch into a solid 3D shape.

## Options

| Option | Description |
| :------ | :----------- |
| Manifold | Ensure the final mesh is manifold. |
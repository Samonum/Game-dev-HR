###Geometry: Scalars, vectors and matrices:

Geometry plays an important part of game development. We need to know where things are and how they relate to one another. Is the player on the ground? did a bullet hit its target, how does an object move? These and many more questions can only be answered with maths.

The basic components we work with are **scalars**, **vectors** and **matrices**.

A **scalar** is a single number, for example *5.6* or *2*. In C# scalars are usually saved as `floats` for numbers with decimals or `ints` if we only care about whole numbers. Scalar values will be written as a single lower case character: $i$.

A **vector** is a list of numbers. The `Vector2` class in monogame for example is a list of two floats. While Vectors can be used for many things, we will mostly use them for locations and directions. For example, the vector $(4, 5)$ points to the coordinate with $x=4$ and $y=5$.

[Insert image]

To distinguish vectors from scalar values we willwrite them with an arrow above them like $\overset{ \rightarrow }{v}$. When revering to the individual coordinates of a vector we use subscript: $v_x$ and $v_y$. Note how these are now scalar values, so they no longer have an arrow.

It is in other literature also common to see vectors written in bold $\mathbf{v}$.

A **Matrix** is a table of data. A 3x3 matrix 



The length of a vector is often written as $\left|\left| \overset{ \rightarrow }{v} \right| \right|$ and can be calculated using the Pythagorian theorem, $lemgth =. \sqrt(x^2 + y^2)$.


# Geometry: Scalars, vectors and matrices:

Geometry plays an important part of game development. We need to know where things are and how they relate to one another. Is the player on the ground? did a bullet hit its target, how does an object move? These and many more questions can only be answered with maths.

The basic components we work with are **scalars**, **vectors** and **matrices**.

## Scalars
A **scalar** is a single number, for example *5.6* or *2*. In C# scalars are usually saved as `floats` for numbers with decimals or `ints` if we only care about whole numbers. Scalar values will be written as a single lower case character: $i$.

## Vectors
A **vector** is a list of numbers. The `Vector2` class in monogame for example is a list of two floats. While Vectors can be used for many things, we will mostly use them for locations and directions. For example, the vector $(4, 5)$ points to the coordinate with $x=4$ and $y=5$.

[Insert image]

To distinguish vectors from scalar values we willwrite them with an arrow above them like $\overset{ \rightarrow }{v}$. When revering to the individual coordinates of a vector we use subscript: $v_x$ and $v_y$. Note how these are now scalar values, so they no longer have an arrow.

It is in other literature it is also common to see vectors written in bold $\mathbf{v}$.

## Matrices
A **matrix** is a table of data. A 3x3 matrix contains 3 rows, with 3 values each. We will use matrices to create specific transformations on vectors, like scaling, rotation and translation. 

```math
I = \begin{bmatrix} 1 & 0 & 0 \\\ 0 & 1 & 0 \\\ 0 & 0 & 1 \end{bmatrix}
```
Matrices are denoted using capital letters like $M$.


## Tensor
A **tensor** is a generalisation of matrices to 3, 4 or even more dimentions. We won't be using any tensors during the course.

# Geometry
Geometry

## Length
The length of a vector is often written as $\left|\left| \overset{ \rightarrow }{v} \right| \right|$ and can be calculated using the Pythagorian theorem:
```math
\left|\left| \overset{ \rightarrow }{v} \right| \right| = \sqrt{{v_x}^2 + {v_y}^2}
```

[insert image]

**Example:** if you have the vector $\overset{ \rightarrow }{v}$ $= (3, 4)$ then we can fill in the above formula to find that:
```math 
\left|\left| \overset{ \rightarrow }{v} \right| \right| = \sqrt{3^2+4^2} = \sqrt{9+16} = \sqrt{25} = 5
```

## Scalar multiplication
You can multiply a vector with a scalar to scale a vector. To multiply a vector with a scalar you simply multiply each of the components of a vector with said scalar:

```math
\overset{ \rightarrow }{w} = s\overset{ \rightarrow }{v} = (sv_x, sv_y)
```

```math
\overset{ \rightarrow }{w} = s\overset{ \rightarrow }{v} \Rightarrow  \left|\left| \overset{ \rightarrow }{w} \right| \right| = s\left|\left| \overset{ \rightarrow }{v} \right| \right|
```

## Unit vectors and normalization
A unit vector is a vector of length 1. As we have seen above, multiplying a vector with a scalar creates a vector who's length is equal to the original vector's length times said scalar. Therefore, you can turn a vector into a unit vector pointing in the same direction by dividing it by its length.

Turning a vector into an unit vector is called normalization. Normalized vectors are often denoted with a ^ above them. 


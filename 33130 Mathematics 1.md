# 33130 Mathematics 1 Notes

* ### Week 1 [Vectors and 3D Space]
    * Revision of Angles
    * 2D and 3D Coordinate Systems
    * Intro to Vectors
    * The Dot Product
    * Scalar and Vector Projections
* ### Week 2 [Vectors and 3D Space cont.]
    *  The Cross Product  
    *  Equation of a Line in 3D
    *  Equation of a Plane in 3D
* ### Week 3 [Matrices]

## Week 1

  ### Revision of Angles
**Radians**  
A radian is a unit of angle, where 1 radian is defined as the angle subtended at the center of a circle by an arc of length equal to the radius.  
There are $2\pi$ radians in a circle, $180^\circ = \pi$ radians, $90^\circ = \frac{\pi}{2}$ radians and so on. Radians are used since they result in more natural results and  
formulas compared to degrees which are relatively arbitrary.  
An example of one such formula is the arc-length formula where the length of an arc $s$ is given by $s = r\theta$ where $r$ is the radius of the circle  
and $\theta$ is the central angle.  

To convert from radians to degrees and visa versa you can use the relation $\frac{\text{radians}}{2\pi} = \frac{\text{degrees}}{360}$ and rearrange to $\text{radians} = \frac{2\pi\cdot\text{degrees}}{360}$ or  
$\text{degrees} = \frac{360\cdot\text{radians}}{2\pi}$ depending on what you are trying to convert to and from.  

**Sine and Cosine**  
Sin and cos are trigonometric functions that have a wide range of uses.  
In a right angled triangle the sin and cos functions can be used to relate the ratios between the lengths of the sides to angles.  
$\cos{\theta} = \frac{\text{adjacent}}{\text{hypotenuse}}$ and $\sin{\theta} = \frac{\text{opposite}}{\text{hypotenuse}}$ where $\text{adjacent}$, $\text{opposite}$ and $\text{hypotenuse}$ are the three sides of the triangle relative to the angle $\theta$.  
  
Sin and cos can also be visualised using a unit circle (circle of radius one, centered at the origin), where the coordinates of a point on the edge of the circle are $(\cos{\theta},\ \sin{\theta})$ for some angle $\theta$, and as $\theta$ goes from $0$ to $2\pi$
the point on the unit circle completes a full revolution counter clockwise, starting and ending at $(1,\ 0)$.  

There are a number of trigonemtric identities which are very useful to know, some of which are below.
* $\sin^{2}{\theta} + \cos^{2}{\theta} = 1$
* $\sin{(A+B)} = \sin{A}\cos{B} + \cos{A}\sin{B}$
* $\cos{(A+B)} = \cos{A}\cos{B} - \sin{A}\sin{B}$
* $\sin{(-x)} = -\sin{x}$
* $\cos{(-x)} = \cos{x}$
* $\sin{x} = \cos{(x-\frac{\pi}{2})}$
---

  ### 2D and 3D Coordinate Systems
**2D Space**  
Two dimensional space is comprised of two axes, generally denoted $x$ and $y$, and are represented as a cartesian plane. Any point on the plane can be represented by these $x$ and $y$ coordinates. That is to say for any ordered pair, $(x,\ y) \in \mathrm{R}^{2}$.
It follows that points in 2D space are written as an ordered pair $(x,\ y)$. To assign a point as a variable, say $A$, most commonly $A = (x_1,\ y_1)$ or $A(x_1,\ y_1)$ are used.  
The distance between two points is given by the formula $d =$ $\scriptstyle \sqrt{(x_2 - x_1)^{2} + (y_2 - y_1)^{2}}$ or alternatively $d = \left|(x_2,\ y_2) - (x_1,\ y_1)\right|$.  
  
**3D Space**  
Similarly, three dimensional space follows all the same principals, just with an added $z$ axis. Every point in 3D space can be represented as an ordered pair $(x,\ y,\ z) \in \mathrm{R}^{3}$ and points are denoted $A = (x_1,\ y_1,\ z_1)$ or $A(x_1,\ y_1,\ z_1)$.
Furthermore the distance between two points in 3D is simply extended to $d =$ $\scriptstyle \sqrt{(x_2 - x_1)^{2} + (y_2 - y_1)^{2} + (z_2 - z_1)^{2}}$ or alternatively $d = \left|(x_2,\ y_2,\ z_2) - (x_1,\ y_1,\ z_1)\right|$.  
  
**Sets of Points**  
A set of points can be used to describe mathematical objects such as lines, or surfaces in 2D and 3D space. They can be defined using the following notation in 2D, $\\{(x,\ y)\ :\ \text{condition}\\}$, or in 3D as, $\\{(x,\ y,\ z)\ :\ \text{condition}\\}$.
Read in natural language as "The set of numbers which obey the following condition". For example the set of points that are a distance of two from the origin in 3D would be $\\{(x,\ y,\ z)\ :\ x^{2} + y^{2} + z^{2} = 4\\}$.  

---

  ### Intro to Vectors
**Vectors**  
Scalar quantities are completely specified by a single pure number whereas vectors are specified by both magnitude and direction.  
Vectors can be represented in a multitude of ways. For example the vector with components $a$, $b$ and $c$ can be represented as:
```math
\begin{align}
    \begin{bmatrix} a \\ b \\ c \end{bmatrix} &\quad \text{column vector} \\
    \langle a, b, c \rangle &\quad \text{bra-ket notation} \\
    \left( a, b, c \right) &\quad \text{ordered triplet} \\
    a \cdot \hat{i} + b \cdot \hat{j} + c \cdot \hat{k} &\quad \text{component form}
\end{align}
```
Some other important things to note when writing vectors as variables, a squiggle is placed either below or above the letter like so, $\overset{\sim}{v}$ or $\underset{\sim}{v}$, alternatively an arrow can be used like so, $\vec{v}$ or $\overrightarrow{AB}$.  
In the component form above $\hat{i}$, $\hat{j}$ and $\hat{k}$ are known as the coordinate axis vectors and have values of $\langle 1, 0, 0 \rangle$, $\langle 0, 1, 0 \rangle$ and $\langle 0, 0, 1 \rangle$ respectively. These vectors form a complete basis
meaning that any vector can be expressed in terms of them.  
A vector can have more than two or three dimensions but for the most part in this course only 2D and 3D vectors will be worked with.  
The magnitude or length of a vector is given by $\left| \underset{\sim}{v} \right| =$ $\scriptstyle \sqrt{v_x^{2} + v_y^{2} + v_z^{2}}$.  

---

  ### The Dot Product
  ### Scalar and Vector Projections

## Week 2

  ### The Cross Product  
  ### Equation of a Line in 3D
  ### Equation of a Plane in 3D

## Week 3

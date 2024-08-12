Taylor Series

 It is the function of an infinite sum of terms in increasing order of degree. Taylor series of **Polynomial** function is a **Polynomial**. 

**_Ex. with respect. to **Taylor Series**_**

Let _f_ be a **function** with derivatives of all orders throughout some interval containing _a_ as an interior point. Then the **Taylor series generated by _f_ at _x=a_ is** 

$$
\displaystyle\sum_{k=0}^{infinity}\frac{f^k(a)}{k!} (x-a)^k= f(a)+ f'(a) (x-a) +\frac{f''(a)}{2!} (x-a)^2 +.... +\frac{f^n(a)}{n!} (x-a) ^n+..., 
$$                                                              
                                                             
 _When the **Taylor series** is centered at **Zero** it is known as **Maclaurin Series**._
 
 The **Maclaurin series generated by _f_ is**
 
 $$
 \displaystyle\sum_{k=0}^{infinity}\frac{f^k(0)}{k!} x^k = f(0)+ f'(0)x+\frac{f''(0) }{2!} x^2x +.... + \frac{f^n(0)}{n!} x^n+..., 
 $$
 
The **Taylor series** generated by _f_ at _x_=0
 

# Question relevant to **Taylor series**
Find the **Taylor series** generated by

$$ 
f(x) = \frac{1}{x}
$$
                                       
at a=2. Where, if anywhere, does the series converge to
                                       
$$
\frac{1}{x} ? 
$$
 
**Solution**
We need to find f(2), f'(2), f''(2),........ Taking derivatives we get

$$ 
\frac{f(2)+ f'(2) (x-2) +\frac{f''(2)}{2!} (x-a)^2 +.... +\frac{f^n}{n!} (x-2) ^n+...,      
$$

    
      
# Chapter 3: Partial Differentiation

## Introduction

The real world can be described in mathematical terms using parametric equations and functions such as trigonometric functions which describe cyclic, repetitive activity; exponential, logarithmic and logistic functions which describe growth and decay and polynomial functions which approximate these and most other functions. The problems in operations research, computer science, probability, statistics, fluid dynamics, economics, electricity, etc. deal with functions of two or more independent variables. In this chapter, we study the limit, continuity, partial derivatives of such functions, Euler's theorem, Jacobians which determine the functional dependence and determination of errors and approximations of calculations.

## 3.1 Functions of Several Variables: Limit and Continuity

The area of an ellipse is πab. It depends on two variables *a* and *b*; The total surface area of a rectangular parallelepiped is 2(xy + yz + zx) and it depends on 3 variables x, y, z; The velocity v of a fluid particle moving in space depends on 4 variables x, y, z, t. In transportation problems in operations research, the cost function to be minimized is a function of several (m: n; running into hundreds) variables (where m is the number of origins and n is the number of destinations). Thus, functions of several variables play a vital role in advanced Mathematics.

### Function of Two Variables

If u = f(x, y, z, t) then x, y, z, t are known as the independent variables or arguments and u is known as the 'dependent variable' or 'value' of the function. In this section, we restrict to functions of two and three variables, although the analysis can easily be extended to several variables.

#### Function of Two Variables

If for every x and y a unique value f(x, y) is associated, then f is said to be a function of the two independent variables x and y and is denoted by:

z = f(x, y)

Geometrically, in three-dimensional xyz-coordinate space (1) represents a surface. The values of x and y for which the function is defined is known as the domain of definition of the function:

**Example:**

z = √(a² - x² - y²)

**Domain:** x² + y² ≤ a²

Function not defined when x² + y² > a².

**Example:**

z = xᵐ + yⁿ

**Domain:** x > 0 and y > 0.

#### δ-neighbourhood of a point (a, b)

The δ-neighbourhood of a point (a, b) in the xy-plane is a square with center at (a, b) bound by the four lines x = a - δ, x = a + δ, y = b - δ, y = b + δ, i.e.,

a - δ ≤ x ≤ a + δ  
b - δ ≤ y ≤ b + δ.      
           
**Note:** Neighbourhood of a point (a, b) may also be defined as a circular disk with center at (a, b) and of radius δ given by

\[
(x - a)² + (y - b)² < δ²
\]

The concept of limit is paramount in defining continuity and differentiability of a function. Note that all three concepts of limit, continuity and differentiability are point concepts i.e., defined at a point.

#### Limit:
A function \( f(x, y) \) is said to have a limit \( L \) as the point \( (x, y) \) approaches \( (a, b) \) and is denoted as

\[
\lim_{{(x, y) \to (a, b)}} f(x, y) = L
\]

if the value of \( f(x, y) \) can be made as close (as we please) to the given finite number \( L \) for all those \( (x, y) \) in an appropriately chosen δ-neighbourhood of \( (a, b) \), i.e., for a given \( \epsilon > 0 \) we can find δ such that

\[
|f(x, y) - L| < \epsilon
\]

for all \( (x, y) \) in the δ-neighbourhood

\[
|x - a| < \delta \quad \text{and} \quad |y - b| < \delta
\]

(or alternatively when \( (x - a)² + (y - b)² < \delta² \)).

**Important Note:** The limit of a function \( f(x, y) \) of two variables is said to exist *only when* the same value is obtained for the limit along any path in the xy-plane from \( (x, y) \) to \( (a, b) \) say along \( x \to a \) and \( y \to b \) or along \( y \to b \) and \( x \to a \), etc.

Limit may or may not exist. If it exists the limit must be unique.

#### Method of Obtaining Limit

- **Step I:** Evaluate \(\lim_{{x \to a}} f(x, y)\) along path I: \( x \to a \) and \( x \to b \).
- **Step II:** Evaluate \(\lim_{{x \to a}} f(x, y)\) along path II: \( y \to b \) and \( x \to a \).

  If the limit values along path I and II are same, the limit exists. Otherwise not.

- **Step III:** If \( a = 0, b = 0 \), evaluate limit along say path \( y = mx² \) also.

**Results:** If 

\[
\lim_{{(x, y) \to (a, b)}} f(x, y) = L
\]

and

\[
\lim_{{(x, y) \to (a, b)}} g(x, y) = M,
\]

then:

1. \(\lim_{{(x, y) \to (a, b)}} (f + g) = L \pm M\)
2. \(\lim_{{(x, y) \to (a, b)}} (f \cdot g) = L \cdot M\)
3. \(\lim_{{(x, y) \to (a, b)}} \left(\frac{f}{g}\right) = \frac{L}{M}, \text{ provided } M \neq 0.\)

#### Continuity

A function \( f(x, y) \) is said to be continuous at a point \( (a, b) \) if 

\[
\lim_{{(x, y) \to (a, b)}} f(x, y) = f(a, b)
\]

i.e., the limit of \( f \) as \( (x, y) \) tends to \( (a, b) \) is the value of \( f \) at \( (a, b) \).

A function is said to be continuous in a domain if it is continuous at every point of the domain. Equation (2) can also be written as 

\[
\lim_{{(x, y) \to (a, b)}} f(a + h, b + k) = f(a, b)
\]

If \( f \) is not continuous at \( (a, b) \), it is said to be discontinuous at \( (a, b) \).

**Result:** If \( f(x, y) \) and \( g(x, y) \) are continuous at \( (a, b) \), then \( f \pm g \), \( f \cdot g \) and \( \frac{f}{g} \) are continuous at \( (a, b) \).

#### Test for Continuity at a Point \( (a, b) \)

- **Step I:** \( f(a, b) \) should be well defined.
- **Step II:** \(\lim_{{(x, y) \to (a, b)}} f(x, y) \) should exist (must be unique and same along any path).
- **Step III:** The limit of \( f = \) value of \( f \) at \( (a, b) \).

### Worked Out Examples

**Limits**

**Example 1:** Evaluate \(\lim_{{(x, y) \to (0, 0)}} (x² + y²)\)

**Solution:**

\[
\lim_{{(x, y) \to (0, 0)}} (x² + y²) = 0
\]

Taking \( y = mx \), we get

\[
\lim_{{x \to 0}} (x²(1 + m²)) = 0
\]

Taking \( x = 0 \), we get

\[
\lim_{{y \to 0}} y² = 0
\]

Similarly, taking \( y = 0 \), we get

\[
\lim_{{x \to 0}} x² = 0
\]
 

#### Along \( y = mx \)
\[
\lim_{x \to 0} \left( x^2 + y^2 \right) = \lim_{x \to 0} \left( x^2 + m^2x^2 \right) 
\]
\[
= \lim_{x \to 0} \left(1 + m^2\right) x^2 = \left(1 + m^2\right) \lim_{x \to 0} x^2 = 0
\]

#### Along \( y = mx^2 \)
\[
\lim_{x \to 0} \left( x^2 + y^2 \right) = \lim_{x \to 0} \left( x^2 \left(1 + m^2x^2 \right) \right) = 0
\]
Since the value of the limit along any path is the same, the limit exists and the limit value is zero.

**Example 2:** If \( f(x, y) = \frac{y^2 - x^2}{x^2 + y^2} \), show that
\[
\lim_{(x, y) \to (0, 0)} \left| f(x, y) \right| \neq \lim_{(x, y) \to (0, 0)} f(x, y)
\]

**Solution:**

**L.H.S. of the inequality:**

\[
\lim_{x \to 0} \lim_{y \to 0} \left| f(x, y) \right| = \lim_{x \to 0} \lim_{y \to 0} \left| \frac{y^2 - x^2}{x^2 + y^2} \right| = \lim_{x \to 0} \frac{x^2 - x^2}{x^2 + y^2}
\]

\[
= \lim_{x \to 0} \frac{x^2}{x^2} \times \lim_{y \to 0} 1 - 1 = 1 - 1 = 0
\]

**R.H.S. of the inequality:**

\[
\lim_{y \to 0} \lim_{x \to 0} \left| f(x, y) \right| = \lim_{y \to 0} \lim_{x \to 0} \frac{y^2 - x^2}{x^2 + y^2} = \lim_{y \to 0} \frac{x^2}{x^2 + y^2}
\]

\[
= \lim_{y \to 0} \left[ \frac{x^2}{x^2 + y^2} \right] = 1 - 1 = 0
\]
Thus L.H.S. \( = -1 \neq 1 = \) R.H.S.  
\[ 
\text{[Note: Since the limits along two different paths are not the same, the limit does not exist.]}
\]

**Example 3:** Evaluate  
\[ 
\lim_{(x, y) \to (0, 0)} \frac{x^2y}{(x^2 + y^2)^2} 
\]

**Solution:**

1. **I.**  
\[
\lim_{y \to 0} \frac{x^2y}{(x^2 + y^2)^2} = \lim_{y \to 0} 0 = 0
\]

2. **II.**  
\[
\lim_{x \to 0} \frac{x^2y}{(x^2 + y^2)^2} = \lim_{x \to 0} 0 = 0
\]

3. **III.**  
\[
\lim_{x \to 0} \lim_{y \to 0} \frac{mx^3}{\left(1 + m^2x^2\right)^2} = \lim_{x \to 0} \frac{mx^3}{\left(1 + m^2x^2\right)^2} = 0
\]

Since the limit along the last path \( y = mx^2 \) depends on \( m \), the limit does not exist.

#### Continuity

**Example 4:** If \( f(x, y) = \frac{x^3y}{x^2 + y^2} \) when \( x \neq 0, y \neq 0 \) and \( f(x, y) = 0 \) when \( x = 0, y = 0 \), find out whether the function \( f(x, y) \) is continuous at origin.

**Solution:** First calculate the limit of the function:

1. **I.**  
\[
\lim_{y \to 0} \frac{x^3y}{x^2 + y^2} = \lim_{y \to 0} 0 = 0
\]

2. **II.**  
\[
\lim_{x \to 0} \frac{x^3y}{x^2 + y^2} = \lim_{x \to 0} 0 = 0
\]

3. **III.**  
\[
\lim_{x \to 0} \lim_{y \to 0} \frac{mx^3y}{\left(1 + m^2x^2\right)^2} = \lim_{x \to 0} \frac{mx^3}{\left(1 + m^2x^2\right)^2} = 0
\]

Since the limit along any path is the same, the limit exists and equal to zero which is the value of the function \( f(x, y) \) at the origin. Hence the function \( f \) is continuous at the origin.

**Example 5:** Discuss the continuity of the function \( f(x, y) = \frac{x^3y}{x^2 + y^2} \) when \( x \neq 0, y \neq 0 \) and \( f(x, y) = 2 \) when \( x = 0, y = 0 \).

**Solution:** At first, evaluate the limit

1. **I.**  
\[
\lim_{y \to 0} \frac{x}{\sqrt{x^2 + y^2}} = 0
\]            
--- 
### 3.4 — HIGHER ENGINEERING MATHEMATICS—II

---

**II.** \(\lim_{x \to 0} \frac{x}{\sqrt{x^2 + y^2}} = \lim_{y \to 0} \frac{x}{\sqrt{x^2}} = \lim_{x \to 0} \frac{x}{|x|} = 1 = 1\)

Since the limits along paths I and II are different, the limit itself does not exist. Therefore the function is discontinuous at the origin.

**Example 6:** Examine for continuity at origin of the function defined by

\[f(x, y) = \frac{x^2}{\sqrt{x^2 + y^2}}\] for \( (x \neq 0, y \neq 0) \)

\[= 3,\text{ for } (x = 0, y = 0)\]

Redefine the function to make it continuous.

**Solution:**

Initially,⬤
Example 6: Examine for continuity at origin of the function defined by:

\[
f(x, y) = \frac{x^2}{\sqrt{x^2 + y^2}}, \text{ for } (x \neq 0, y \neq 0)
\]

Re-define the function to make it continuous.

**Solution:**

- Initially, find the limit:

\[
\lim_{x \to 0} \frac{x^2}{\sqrt{x^2 + y^2}} = 0
\]

Therefore \( f \) is continuous at origin by redefining \( f(0, 0) = 0 \).

**Exercise: Limits**

Evaluate the following limits:

1. \( \lim_{(x,y) \to (0,0)} \frac{x^2 + y^3}{2xy} \)
   - Ans: \( \frac{3}{2} \)

2. \( \lim_{(x,y) \to (0,0)} \frac{x^2 + y^2}{x^2 + y^2} \)
   - Ans: \( 3 \)
Hint: \( \lim y = me, depends on \( m \), so limit does not exist.

Find out (and give reason) whether \( f(x, y) \) is continuous at \( (0, 0) \) if \( f(0, 0) = 0 \) and for \( (x, y) \neq 0 \) the function \( f \) is equal to:

**Exercise 12.** 
- (a) Is the function \( f(x, y) = \frac{xy(x^2 - y^2)}{x^2 + y^2} \) continuous at origin? 
  - Ans: Not continuous; limit does not exist.
- (b) Redefine \( f(0, 0) = 0 \) to make it continuous.
  - Ans: \( f(0, 0) = 0 \), so \( f \) becomes continuous at origin.

**Exercise 13.**
- If \( f(x, y) = x^4 + y^2 \) determine where the function is continuous.
  - Ans: Continuous for all \( x \) and \( y \).

**Exercise 14.**
- If \( f(x, y) = \frac{15xy}{x^2 + y^2} \), show that \( f \) is discontinuous at origin.
  - Ans: Discontinuous at origin.

**Exercise 15.**
- Given \( f(x, y) = x^3 + 3y^2 + 2x \) for every \( x, y \) except at \( (2, 3) \), determine if it is continuous at \( (2, 3) \).
  - Ans: Discontinuous at \( (2, 3) \), redefined as \( f(2, 3) = 42 \).

---
![Figure 3.1](#)

We can have: 

\[
\frac{\partial u}{\partial y} = \frac{\partial f}{\partial y} = f_y, \quad \frac{\partial u}{\partial x} = \frac{\partial f}{\partial x} = f_x
\]

The value of a partial derivative at a point \((a, b, c)\) is denoted by:

\[
\frac{\partial u}{\partial x}\bigg|_{x=a, y=b, z=c} = \frac{\partial u}{\partial x}(a, b, c) = f_x(a, b, c)
\]

**Geometrical interpretation of a partial derivative of a function of two variables**: \(z = f(x, y)\) represents the equation of a surface in \(xyz\)-coordinate system. Let APB the curve, which a plane through any point \(P\) on the surface parallel to the \(xz\)-plane, cuts. As point \(P\) moves along this curve APB, its coordinates \(z\) and \(x\) vary while \(y\) remains constant. The slope of the tangent line at \(P\) to APB represents the rate at which \(z\) changes w.r.t. \(x\).

Thus:

\[
\frac{\partial z}{\partial x} = \tan \alpha = \text{slope of the curve } APB \text{ at the point } P
\]

Similarly,

\[
\frac{\partial z}{\partial y} = \tan \beta = \text{slope of the curve } CPD \text{ at } P
\]

#### Higher Order Partial Derivatives

Partial derivatives of higher order, of a function \(f(x, y, z)\) are calculated by successive differentiation.

Thus if \(u = f(x, y, z)\) then:

\[
\frac{\partial^2 u}{\partial x \partial y} = \frac{\partial^2 f}{\partial x \partial y} = \frac{\partial}{\partial x} \left(\frac{\partial f}{\partial y}\right) = f_{xy} = f_{12}
\]

And similarly for other higher-order derivatives.

Note 1: The crossed or mixed partial derivatives \(\frac{\partial^2 u}{\partial y \partial x}\) and \(\frac{\partial^2 u}{\partial x \partial y}\) are in general equal.

\[
\frac{\partial^2 f}{\partial x \partial y} = \frac{\partial^2 f}{\partial y \partial x}
\]

Note 2: In the subscript notation, the subscripts are written in the same order in which differentiation is carried out.

Note 3: A function of two variables has two first-order derivatives, four second-order derivatives, and two \(n^{th}\) order derivatives.

#### Worked Out Examples

**Example 1:** Find the first-order partial derivatives \(\frac{\partial u}{\partial x}\) and \(\frac{\partial u}{\partial y}\) when:

a) \(u = e^{x \cos y}\)

b) \(u = \tan^{-1} \frac{y}{x}\)

c) \(u = \ln \left(x^2 + y^2\right)\)

---
### PARTIAL DIFFERENTIATION — 3.7

#### Solution:

**a.**

\[
\frac{\partial w}{\partial x} = \cos y \frac{\partial}{\partial x}(e^x) = e^x \cos y
\]

\[
\frac{\partial w}{\partial y} = e^x \frac{\partial}{\partial y}(\cos y) = -e^x \sin y
\]

**b.**

\[
\frac{\partial w}{\partial x} = \frac{1}{1 + \left(\frac{x}{y}\right)^2} \cdot \frac{\partial}{\partial x} \left(\frac{y}{x}\right) = \frac{-y}{x^2 + y^2}
\]

\[
\frac{\partial w}{\partial y} = \frac{1}{1 + \left(\frac{x}{y}\right)^2} \cdot \frac{\partial}{\partial y} \left(\frac{x}{y}\right) = \frac{x}{x^2 + y^2}
\]

**c.**

\[
\frac{\partial w}{\partial x} = \frac{1}{\sqrt{x^2 + y^2}} \cdot \frac{1}{2 \sqrt{x^2 + y^2}} \cdot \frac{\partial}{\partial x} \left( x^2 + y^2 \right) = \frac{x}{\sqrt{x^2 + y^2}}
\]

\[
\frac{\partial w}{\partial y} = \frac{1}{\sqrt{x^2 + y^2}} \cdot \frac{1}{2 \sqrt{x^2 + y^2}} \cdot \frac{\partial}{\partial y} \left( x^2 + y^2 \right) = \frac{y}{\sqrt{x^2 + y^2}}
\]

---

### Example 2:

Find the partial derivative of \( f \) with respect to each of the independent variables:

**a.**

\[
f(x, y, z, w) = x^2e^{2y+3z} \cos(4w)
\]

\[
f_x = \frac{\partial f}{\partial x} = 2x e^{2y+3z} \cos(4w)
\]

\[
f_y = 2x^2 e^{2y+3z} \cos(4w) \cdot 2
\]

\[
f_z = 2x^2 e^{2y+3z} \cos(4w) \cdot 3
\]

\[
f_w = 2x^2 e^{2y+3z} \cdot -\sin(4w) \cdot 4
\]

**b.**

\[
f(r, \theta, z) = r(2 - \cos 2\theta) / (r^2 + z^2)
\]

\[
\frac{\partial f}{\partial r} = \frac{(r^2 - r^2)(2 - \cos 2\theta) - r(2 - \cos 2\theta) \cdot 2r}{(r^2 + z^2)^2}
\]

---

### Example 3:

Find \( \frac{\partial^3 u}{\partial x \partial y \partial z} \) if \( u = e^{x^2 + y^2 + z^2} \)

**Solution:**

\[
\frac{\partial u}{\partial x} = 2xe^{x^2 + y^2 + z^2}
\]

\[
\frac{\partial^2 u}{\partial y \partial x} = 4xy e^{x^2 + y^2 + z^2}
\]

\[
\frac{\partial^3 u}{\partial z \partial y \partial x} = 8xyz e^{x^2 + y^2 + z^2}
\]

Thus

\[
\frac{\partial^3 u}{\partial x \partial y \partial z} = 8xyz e^{x^2 + y^2 + z^2}
\]

---

### Example 4:

Show that \( V(x, y, z) = \cos 3x \cos 4y \sinh 5z \) satisfies Laplace's equation

\[
\frac{\partial^2 V}{\partial x^2} + \frac{\partial^2 V}{\partial y^2} + \frac{\partial^2 V}{\partial z^2} = 0
\]

**Solution:**

\[
V_{xx} = -3 \sin 3x \cdot \cos 4y \cdot \sinh 5z
\]

\[
V_{yy} = -16 \cos 3x \cdot \sin 4y \cdot \sinh 5z
\]

\[
V_{zz} = 25 \cos 3x \cdot \cos 4y \cdot \sinh 5z
\]

Adding (1), (2), and (3), we get

\[
V_{xx} + V_{yy} + V_{zz} = 0
\]

---

### Example 5:

If \( u = e^{\alpha t} \cos(a \ln r) \), show that

\[
\frac{\partial^2 u}{\partial r^2} + \frac{1}{r} \frac{\partial u}{\partial r} + \frac{1}{r^2} \frac{\partial^2 u}{\partial \theta^2} = 0
\]
### 3.8 HIGHER ENGINEERING MATHEMATICS—II

#### Solution:

\[
u = e^{\alpha t} (\text{cos }a \ln r) \quad (1)
\]

\[
u_{rr} = e^{\alpha t} \left[ \frac{-1}{r^2} \sin(a \ln r) + \frac{\cos(a \ln r)}{r^2} \right] \quad (2)
\]

\[
u_{\theta\theta} = -ae^{\alpha t} \sin(a \ln r) \quad (3)
\]

\[
u_{t} = \alpha e^{\alpha t} \cos(a \ln r) \quad (4)
\]

using (1), (2), and (3)

\[
u_{rr} + \frac{1}{r^2}u_{\theta\theta} = e^{\alpha t} \left[\frac{ae^{\alpha t}}{r^2} \sin(a \ln r) - \frac{a^2}{r^2} \right] + \left(- \frac{ae^{\alpha t}}{r^2} \sin(a \ln r)\right) + \left(\frac{\alpha^2 e^{\alpha t}}{r^2}\right) = 0
\]

#### Example 6: 

If \( u = \ln(x^3 + y^3 - \frac{x^2y - xy^2}{x^2+y^2}) \), then show that \( u_{xx} + 2u_{xy} + u_{yy} = 0 \)

**Solution:**

\[
u_x = \frac{3x^2 - 2xy - y^2}{(x^3 + y^3 - x^2y - xy^2) - \frac{xy(x+y)}{(x^2 + y^2)}} \quad (1)
\]

\[
u_y = \frac{3y^2 - 2xy - x^2}{(x^3 + y^3 - x^2y - xy^2) - \frac{xy(x+y)}{(x^2 + y^2)}} \quad (2)
\]

Adding (1) and (2), we get

\[
u_x + u_y = \frac{(3x^2 - 2xy - y^2) + (3y^2 - 2xy - x^2)}{(x^3 + y^3 - x^2y - xy^2)} = \frac{2(x+y)(x-y)}{x^2 + y^2} + 2xy \quad (3)
\]

Now

\[
u_{xx} + 2u_{xy} + u_{yy} = \frac{\partial^2 u}{\partial x^2} + 2 \frac{\partial^2 u}{\partial x \partial y} + \frac{\partial^2 u}{\partial y^2} = 0
\]

---

### EXERCISE

1. Find the first order partial derivatives of:
    - a. \( u = x+y \)
    - b. \( u = \ln(x + \sqrt{x^2 - y^2}) \)
    - c. \( u = \sin y \)
    - d. \( u = x^y \)

**Ans.**
- a. \( u_x = 1 \), \( u_y = 1 \)
- b. \( u_x = \frac{1}{x + \sqrt{x^2 - y^2}} \times \left(1 + \frac{x}{\sqrt{x^2 - y^2}}\right) \), \( u_y = \frac{-y}{(x + \sqrt{x^2 - y^2}) \sqrt{x^2 - y^2}} \)
- c. \( u_x = 0 \), \( u_y = \cos y \)
- d. \( u_x = yx^{y-1} \log x \), \( u_y = x^y \log x \)

2. Find the partial derivative of the given function w.r.t. each variable:
    - a. \( f(x, y, z) = \sin^{-1}(y/z) \)
    - b. \( f(x, y, u, w) = (u^2 - w^2)\sin^{-1}(y/x) \)
    - c. \( f(x, y, r, s) = \sin 2x \sin 3y \cos 4s \)
    - d. \( f(x, y, r, s) = 4\sin 3y \sin 4s \)

**Ans.**
- a. \( f_x = 0 \), \( f_y = \frac{1}{z} \), \( f_z = \frac{-y}{z^2 \sqrt{1 - y^2/z^2}} \)
- b. \( f_u = 2u \sin^{-1}(y/x) \), \( f_w = -2w \sin^{-1}(y/x) \)
- c. \( f_r = 2 \cos 2x \cos 3r \), \( f_s = 3 \cos 3y \cos 4s \)
- d. \( f_r = 3 \sin 2r \sin 3r \), \( f_s = 4\sin 3y \sin 4s \)

3. If \( w = \ln(2x + 2y) \text{ and } u = 2x(y - 2y) \), prove that 

\[
\frac{\partial^2 w}{\partial x \partial y} = \frac{\partial^2 w}{\partial y^2}
\]
 ## PARTIAL DIFFERENTIATION — 3.9

4. Verify that \( w_{xy} = w_{yx} \) when 
   a. \( u = \ln(2x + 3y) \)
   b. \( w = x^3y^2 + 3x^2y^4 \)
   c. \( w = \tan^{-1} \frac{y}{x} \)
   d. \( w = \ln(x \sin x + \sin y) \)

5. Show that \( u_x + u_y = u \) if \( u = e^{x+y}/(e^x + e^y) \).

6. Prove that \( w = f(x + ct) + g(x - ct) \) satisfies the wave equation \( \frac{\partial^2 w}{\partial t^2} = c^2 \frac{\partial^2 w}{\partial x^2} \) where c is a constant. Verify this when
   \( w = 7\sin(3x + 5ct) + 9\cosh(5x - 5ct) \).

7. Show that \( w_{xx} + w_{tt} = 0 \) if
   \( w = \sin(2x - 3ct) \).

8. If \( w = x^4 + y^4 + z^4 + 2xyz \), prove that
   \( w_{xx} + w_{yy} + w_{zz} = 6(x + y + z) \).

9. Verify that V satisfies Laplace's equation
   \[
   \frac{\partial^2 V}{\partial x^2} + \frac{\partial^2 V}{\partial y^2} + \frac{\partial^2 V}{\partial z^2} = 0
   \]
   if (a) \( V = x^2 + y^2 - 2z^2 \), (b) \( V = e^{x^2 + 4y} \cos 5z \), 
   (c) \( V = \ln(x^2 + y^2 + z^2) \).

10. Find \( \frac{\partial^3 u}{\partial x \partial y \partial z} \) if \( u = e^{xyz} \).

11. Show that \( w_{xx} + w_{yy} + w_{zz} = 0 \) when
    \[
    w = \frac{y}{x} + \frac{z}{x} + \frac{x}{y} + \frac{z}{y} + \frac{x}{z} + \frac{y}{z}
    \]

12. If \( u = r^m \) prove that
    \[
    u_{xx} + u_{yy} + u_{zz} = m(m + 1)r^{m - 2}
    \]
    where \( r^2 = x^2 + y^2 + z^2 \).

13. For \( m = 2\) or \( 3\) show that \( u = r^m(3 \cos^2 \theta - 1) \) satisfies the differential equation
    \[
    \frac{\partial}{\partial r} \left( r^2 \frac{\partial u}{\partial r} \right) + \frac{1}{\sin \theta} \frac{\partial}{\partial \theta} \left( \sin \theta \frac{\partial u}{\partial \theta} \right) = 0
    \]

14. Prove that \( \left( \frac{\partial^2 u}{\partial r^2} + \frac{1}{r} \frac{\partial u}{\partial r} + \frac{1}{r^2} \frac{\partial^2 u}{\partial \theta^2} \right) = 0 \) if
    \[
    u = \ln(x^2 + y^2) + \left( x + \frac{1}{x^2 + y^2} \right)
    \]

   **Hint:** Prove and use the result \( u_x + u_y + u_z = \left( \frac{1}{x + y + z} \right) \).

15. Prove (the Cauchy-Riemann equations in polar coordinates) \( r u_r = v_{\theta}, r v_r = -u_{\theta} \) when
    \[
    u = r \cos (\cos r), \quad v = r \sin (\sin \theta)
    \]

16. Show that \( v_{xx} + v_{yy} - x^2 - y^2 \).

17. **Hint:** Solve for \( z = (y^2 - x^2) \ln (x - y) \).
    If \( u = (x^2 + y^2) \ln (x - y) \).

18. Prove that \( f(x, t) = a \sin bx \cdot \cos bt \) satisfies
    \[
    \frac{\partial^2 f}{\partial t^2} = c^2 \frac{\partial^2 f}{\partial x^2}
    \]
    where \( c = b \).

19. Show that \( u_x + u_y = 0 \) if \( u = x - y \).

 
     

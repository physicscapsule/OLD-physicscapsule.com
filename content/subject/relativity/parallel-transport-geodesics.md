---
title: "Parallel transport and Geodesics"
author: V.H. Belvadi
---

Moving along the curvature of space that is not Cartesian—or flat—is different from moving along flat space. Although we live on a ‘curved’ Earth we tend not to notice this because our movements are governed by the local flatness of the Earth, i.e. the idea that a sufficiently small region on the Earth can be considered perfectly flat.

If you move across larger regions on the Earth, for example while flying across continents, the familiar flat-space movements do not hold and special movements along curved space come into play. This is just as true for even larger regions, such as traveling across points in our universe—or through spacetime as we call it—as the Earth, Sun and all known planets and stars are doing right now.

Our aim then is a rather fundamental one: we would like to establish an equation that, much like a straight-line takes us from point-to-point on flat space, will take us from point to point in curved space. Such a path, like a straight-line in flat space, has to be the most efficient (read, shortest) path between those two points. We call such a path a Geodesic. And the construction that governs how one moves around in curved space is known as 'Parallel transport'.

# Parallel transport

Consider a curve $ \vec{U} $ parametrised by $ \lambda $. That is to say, consider a curve, every point on which may be mapped onto a certain function, or parameter, called $ \lambda $. If we draw a vector at some point on this curve the method in which we would have to **parallel transport** said vector is to move it by an inifinitesimal distance to a new position, still on the same curve, while keeping it parallel to its old position and of the same length/magnitude. Parallel transport, therefore, is always done with respect to a well-defined curve which might—and often does—happen to be the curvature of spacetime itself.

Based on the above relation between the curve and our parameter, let us define $ \vec{U} = \textrm{d}\vec{x}/\textrm{d}\lambda $ or, equivalently, $ U^\beta = \textrm{d}x^\beta/\textrm{d}\lambda $ as the tangent to the curve $ \vec{U} $.

Also, at some point $ X $, since the vector $ \vec{V} $ remains constant along the curve parametrised by $ \lambda $ as a necessary condition for parallel transport, we have $ \textrm{d}V^\alpha/\textrm{d}\lambda = 0 $ or, combining the above results,

<div>
\begin{align*}
{\textrm{d} V^\alpha \over \textrm{d} \lambda} &= {\textrm{d} V^\alpha \over \textrm{d} x^\beta} {\textrm{d} x^\beta \over \textrm{d} \lambda} \\
&= U^\beta V^\alpha_{; \beta} \tag{1} \label{eq:parallel-transport}
\end{align*}
</div>

where the semicolon subscript denotes a curved space analogue of the familiar flat space derivative with respect to the index that follows it i.e. in the equation above the semicolon derivative represents the curved space analogue of $\textrm{d}V^\alpha/\textrm{d}x^\beta$. Mathematically, given $\textrm{d}V^\alpha/\textrm{d}x^\beta$ the semicolon derivative is defined as

<div>
\begin{equation}
V^\alpha_{; \beta} = V^\alpha_{, \beta} + \Gamma^\alpha_{\mu \beta} V^\mu \tag{2} \label{eq:derivative}
\end{equation}
</div>

where

<div>
\begin{equation}
\Gamma^\alpha_{\mu \beta} = {1\over 2}g^{\alpha\nu} \left( g_{\nu\mu , \beta} + g_{\nu\beta , \mu} - g_{\mu\beta , \nu} \right) \tag{3} \label{eq:gamma}
\end{equation}
</div>

is a Christoffel symbol and $V^\alpha_{, \beta}$ is simply $\textrm{d}V^\alpha/\textrm{d}x^\beta$.

Equation \eqref{eq:parallel-transport} is the mathematical definition of the parallel transport operation of a vector $ \vec{V} $ along a curve $ \vec{U} $. For convenience we sometimes write this as $ \nabla_{\vec{U}} \vec{V} = 0$.

# Geodesics

Parallel transport is only half the picture. While this technique, or construction, is extremely useful in relativity, there is an arguably more useful entity known as a Geodesic which arises from parallel transport that is central to curved space geometry.

In flat space we know that the shortest distance between two points is a straight-line. Mathematically, a straight-line is one whose tangent remains constant over space. That is to say, if I drew the tangent to a straight-line at some point along the line, it would be exactly equal to a tangent drawn similarly but at another point on the same line. In effect we are *parallel transporting* the tangent.

What if we apply this to curved space in an attempt to generalise it? Say we had a curve and we parallel transported an arbitrary tangent to said curve along the curve itself. What we would get, *so long as we drew a curve such that its parallel transported tangent remained the same throughout the curve*, would be analogous to a straight-line in flat space in that it would be the shortest distance between two points in curved space. Such lines are called **geodesics**.

Just as we parallel transported a random vector on a curve above we will now parallel transport a tangent to the curve along the curve itself, i.e. we will solve $\nabla_{\vec{U}} \vec{U} = 0$. From eq. \eqref{eq:parallel-transport}, \eqref{eq:derivative} and \eqref{eq:gamma} we have

<div>
\begin{align*}
U^\beta U^\alpha_{; \beta} &= 0 \\
U^\beta U^\alpha_{, \beta} + \Gamma^\alpha_{\mu\beta} U^\mu U^\beta &= 0 \\
{\textrm{d}x^\beta \over \textrm{d}\lambda} {\textrm{d} \over \textrm{d}x^\beta} {\textrm{d}x^\alpha \over \textrm{d}\lambda} + \Gamma^\alpha_{\mu\beta} {\textrm{d}x^\mu \over \textrm{d}\lambda} {\textrm{d}x^\beta \over \textrm{d}\lambda} &= 0
\end{align*}
</div>

which gives us

<div>
\begin{equation}
\boxed{ {\textrm{d}^2x^\alpha \over \textrm{d}\lambda^2} + \Gamma^\alpha_{\mu\beta} {\textrm{d}x^\mu \over \textrm{d}\lambda} {\textrm{d}x^\beta \over \textrm{d}\lambda} = 0 } \tag{4} \label{eq:geodesic}
\end{equation}
</div>

This is the equation of a geodesic. Knowing the initial conditions, i.e. the conditions at $ \lambda = \lambda_0 $ of $ x^\alpha_0 \equiv x^\alpha (\lambda_0) $ and $ U^\alpha_0 = \left( \textrm{d}x^\alpha/\textrm{d}\lambda \right)\_{\lambda_0} $ we can find a unique geodesic based on eq. \eqref{eq:geodesic}.

The geodesic equation is really four in number, one for each value of $ \alpha $, much like any vector equation that, when written in component form, becomes three in number. Think of the geodesic equation as a sort of equation of motion. An object, left to its wits, will follow the geodesic on any curve. If this sounds unnatural, recall that this is precisely what Newton said except for flat space: [Newton's first law of motion](/subject/classical-mechanics/newtons-first-law) says an object will continue along a straight-line path (the 'geodesic' of flat space) unless some unbalance force prevents this. It is perfectly natural then that the same should hold for a geodesic in curved space.

# Newtonian gravity

It is always helpful to draw parallels, where reasonable, between heavily mathematical ideas and more intuitive notions. In this case that would be general relativity and Newtonian gravity, after all it was Newton's theory that had shaped our idea of gravity for centuries before Einstein.

We begin by asking how the geodesic equation fits into all this. We will have to skip ahead to the weak field metric from Einstein's Field Equations. From this, for now, let us take for granted that

<div>
$$
\textrm{d}s^2 = \left( 1- {2GM\over c^2r} \right) c^2\textrm{d}t^2 - \textrm{d}r^2 - r^2\textrm{d}\phi^2
$$
</div>

where the first term represents the $(0,0) \equiv (t,t)$ component of $g_{\alpha\beta}$, the second represents the $(1,1) \equiv (x,x)$ component and so on. Since it is larger than all other terms by a whopping $c^2$ we can ignore the rest and write down the Christoffel symbol as

<div>
$$
\Gamma^r_{tt} = {1\over 2}g^{rr} \partial_r g_{tt} = {GM \over r^2}
$$
</div>

We can now substitute the above two results into the geodesic equation (eq. \eqref{eq:geodesic}) noting that $x^\alpha \equiv r$, $\lambda \equiv s$, $x^\mu = x^\beta \equiv t$ since $\\Gamma^\alpha\_{\mu\beta} = \Gamma^r\_{tt}$. Consequently arrive at,

<div>
\begin{align}
{\textrm{d}^2 r \over \textrm{d}s^2} + \Gamma^r_{tt} \left( {\textrm{d}t\over\textrm{d}s} \right)^2 = 0
\end{align}
</div>

Since we are in a weak gravitational field it is clear that our object travels really slowly so that even when time passes, not much spatial coverage takes place i.e. the spacetime interval $\textrm{d}s^2 \approx \textrm{d}t^2 + 0$ where $0 = \sum_{i=1}^3 \textrm{d}x^{i^2}$. In other words $\textrm{d}t/\textrm{d}s \approx 1$ in both terms (even in the second-order derivative that we have) and we are left with

<div>
\begin{align}
{\textrm{d}^2 r \over \textrm{d}t^2} + {GM\over r^2} = 0
\end{align}
</div>

which is exactly Newton's law of gravity:

<div>
\begin{align*}
{\textrm{d}^2 r \over \textrm{d}t^2} &= - {GM\over r^2} \\
m\mathbf{a} &= - {GMm\over r^2} \\
\implies \mathbf{F} &= -{GMm \over r^2}
\end{align*}
</div>

Describing a geodesic is therefore natural in general relativity and is in complete agreement with the classical theories that have served us well in their own right.

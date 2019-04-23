---
title: "Newton's Second Law"
date: 2019-04-12T14:01:11+05:30
---

# Newton's second law

We previously discussed how [Newton's first law](/mechanics/newton-first-law-mass-inertia) introduces the concepts of (index: Inertia) and (index: Mass). This law too follows similar steps and—instead of continued rest or motion in the presence of net balanced forces—talks of what happens when the forces acting on an object are unbalanced.

Newton's second law can be stated in two ways, each as important as the other because of the different ideas they give rise to: acceleration and momentum. In terms of acceleration, the law finds its simplest form. It talks of how a force causes a body to experience acceleration.

> The net force acting on a body produces a proportional acceleration.

Note that with both force and acceleration being vector quantities the word 'proportional' refers to consistent change in both direction and magnitude between the two quantities. However, as we will quickly see, Newton's second law as stated above is really a derived form of the original statement, based on momentum, which says —

> The net force on an object is equal to and in the direction of the rate of change of its linear momentum.

The two forms of this law are extremely similar in spirit. This arises mainly as a result of Newton's laws (and all of classical mechanics) being built around systems with constant mass, i.e. within a given situation and for any length of time, with all other parameters being equal, the mass of an object remains unchanged. It is worth noting that any change occurs in terms of weight (a force) as a result of a varying rate of gravitational acceleration, but never in terms of mass.

# Momentum

Although we saw the acceleration definiton first, we will be looking at the second form given its mathematical universality. (The first form, that of acceleration, can be derived from it as we will see later.)

Let us call our force F, our object's mass m and let us assume it moves as a result of this force (see [Newton's first law](/newton-first-law-mass-inertia)) proportional to a velocity v. It is important to understand why we use the term proportional: the body actually accelerates, as we will see, hence its motion will be an acceleration of, say, a, proportional to its velocity v, i.e. as velocity increases, so does its acceleration and vice versa.

{{<figure caption="A force $ \vec{F} $ acting on a mass m and causing it to accelerate at $ \vec{a} $." src="/images/newton-second-law.png">}}

Then, following the second form of the law stated above, we realise that the momentum, $p$, of this body, defined as a product of its mass and velocity at any time t, is proportional to the force. In other words, we know the definition of linear momentum as, $$\begin{equation}\mathbf{P}=\mathit{m}\mathbf{v}\label{eq:Pmv}\end{equation} $$

In exactness, the rate of change of this momentum (i.e. its derivative) is equal to the force applied. And when we say equal, the force and momentum being vectors, we also refer to their common direction.

Mathematically, we could write them as, $$ \begin{align\*} \mathbf{F} = \frac{\textrm{d} \mathbf{P}}{\textrm{d} t} \end{align\*}$$

Using eq. $\eqref{eq:Pmv}$ and the constancy of mass in classical mechanics (as previously mentioned) we arrive at, $$ \begin{align\*} \mathbf{F} = \frac{\textrm{d} m\mathbf{v}}{\textrm{d} t} = m{\textrm{d}\mathbf{v} \over \textrm{d} t} \end{align\*} $$

The rate of change of velocity, v, signified by the derivative on the right hand side, is merely acceleration, a, since $\textrm{d}\mathbf{v}/\textrm{d} t=\mathbf{a}$. $$ \begin{align} \mathbf{F} & = m \mathbf{a} \label{eq:F=ma} \end{align} $$

Equation $\eqref{eq:F=ma}$ is the mathematical form of Newton's second law and establishes an important relationship between F, m and a. Specifically,

- The heavier the body, the greater the force needed to accelerate it,
- The greater the force applied, the faster a body accelerates, and,
- The direction in which the body accelerates is the same as the force that accelerates it.

These are important implications of Newton's second law, proven, but which might appear obvious even without the mathematics. Note, however, that F is really $\mathbf{F}\_{net}$, the net force acting on the body, which must be a non-zero quantity. If it is zero, the first law comes into picture.

# Impulse

Closely related to everything we just saw is the concept of impulse — force that acts over some period of time, $\Delta t$. The phrase, "over a period of time", signals the need for some integration. Hence, for impulse $J$, we may write, $$\begin{align\*} \mathbf{J}=\int^{t=\Delta t}\_{t=0} \mathbf{F} d \mathit{t} \end{align\*} $$

which reduces to, $$ \begin{equation} \mathbf{J}=\int^{t=\Delta t}\_{t=0} \frac{\textrm{d} \mathit{m}\mathbf{v}}{\textrm{d} t} \textrm{d} t = m \textrm{d} \mathbf{v} \end{equation} $$

This gives the concept of an impulse based on Newton's second law.

Alternately, $$ \begin{align\*} \mathbf{F} &= m \mathbf{a} \\ &= m \frac{d \mathbf{v}}{d t} \\ \mathbf{F} d t = \mathbf{J} &= m d \mathbf{v} \end{align\*} $$

The $\mathbf{F} \textrm{d} t = m \textrm{d} \mathbf{v}$ form to work on impulses is used more often for its simplicity.

- - - - - -

## Rockets and other problems

One less observed constraint of Newton's second law is variant mass. Although we have said that an object's mass remains constant over time, the mass of systems may change.

An often stated example is rocket propulsion. The error here it to look at a rocket as an object rather than a system. A rocket is really a system with, at the very least, two  masses: the frame and the fuel. Over time as fuel is burnt or segments are ejected the mass of the system (not object) reduces. This is why Newton's second law cannot be applied here.

We can, of course, always apply it as a sum of parts, which would be an indirect method. It would be pretty much the same with all such systems: seed ploughing machines, paint cans being thrown etc.

## A newton—the unit

Since this second law, unlike the first, actually defines a force $ \mathbf{F} = m  \mathbf{a} $ now would be a good time to talk about the unit of force.

Common sense rightly dictates that the unit of force must be kg m s$^{-1}$, the product of the units of mass and acceleration. However, a special name has been given to that in honour of Newton as the Newton. It may be abbreviated as N, and, since it is the name of a person, has no plural form.

> A newton is the amount of force required to accelerate a 1 kg mass by 1 ms$^{-2}$.

So much for Newton's second law. We find it everywhere: while walking, while driving, while sitting, standing — it is what holds every macroscopic thing on earth, for instance. Next time, we will see Newton's third law.

---
title: "Impact parameter"
date: 2019-05-02T16:40:01+05:30
---


When two objects collide, they apply forces on one another and in general deflect from their original paths. The nature of such a deflection depends on what kind of forces are at play during the collision. And the extent of the deflection is decided by the direction in which the objects moved (straight towards one another for a head-on collision or at some oblique angle) and how fast they travelled when they set off towards one another. A very useful quantity in this regard, that'll help us know the extent of a possible deflection, even before the collision occurs, is the **impact parameter**.

# Collision terminologies
Of the two colliding objects, we assume one of them (usually the more massive one) to be stationary and call it the **target**. The other object headed towards the target will be called the **projectile**. In case of a comet approaching the Sun, the Sun is the target and the comet, the projectile. If a nucleus is being bombarded with a high energy proton, the nucleus is the target and the proton, the projectile.

Firstly, collision as in what we discuss here is slightly different from our intuitive idea of a collision. We tend to think that two objects are said to collide only when they come in contact with one another. This is of course true in case of two billiard balls colliding. But in more subtle cases such as the comet closing in on the Sun, even if the comet misses the Sun and gets deflected due to the Sun's gravity, we say a collision has occurred. The comet needn't necessarily hit the Sun's surface. Similarly, when a proton is accelerated towards a nucleus, the very meaning of contact becomes fuzzy (the particles don't have well defined boundaries) and so we say a collision has occurred between the two if we observe the proton veering off course (or even bouncing back). 

There are broadly two types of collisions: **elastic** and **inelastic**. The collision is elastic if initially the target was at rest and the projectile started off with some kinetic energy, and we find that after the collision, the total kinetic energy of the deflected projectile and the recoiling target equal the initial kinetic energy of the projectile. In short, the kinetic energy is conserved in such collisions. The other type of collision is the inelastic collision - the projectile loses some or all of its kinetic energy in the form of heat generated during the collision. The total energy is still conserved but not the kinetic energy alone.

# The definition
We suppose it should be obvious that the angle by which the projectile deflects on collision with the target, will be large if the projectile was aimed more directly towards the target (a 180 degree bounce back if it was aimed at exactly the centre of the target). We will now see how we can measure how well a projectile is aimed at the target. Firstly, we assume that the projectile is initially very far from the target and hence the target has almost no influence on it. The projectile drifts freely towards the target along a straight line. It begins curving only when it is considerably near the target. We can trace out the path the projectile will take. Let us now draw a straight line parallel to the initial straight line path of the projectile, passing through the centre of the target. The shortest distance between these two lines is what we call the **impact parameter**.

Another way to visualise this is to think in terms of what path the projectile would take if the forces on it due to the target are completely switched off. It would continue to the drift along a straight line and if it missed the target, it would remain undeflected. Then we could say the impact parameter is the distance of closest approach of the projectile.

So it must be clear that a larger impact parameter will mean that the projectile will probably miss the target and if it gets deflected due to a force field, the angle by which it does so will be small. Whereas, if the impact parameter is zero, it means the projectile is headed straight towards the centre of the target and we must expect a head-on collision. It should be noted that the impact parameter must be measured where the projectile is almost free from the influence of the target and moves in a straight line, otherwise we won't have a single value for it - for repulsive deflections, the distance between the projectile path and the line through the centre of the target will constantly increase and vice versa for attractive deflections. 

# Hard sphere scattering
Let us now consider the collision between a point projectile and a hard sphere (the target) of radius $R$. We assume there is no force field between them and hence the projectile either hits the target or misses it. Before the collision, the projectile is completely free and drifts along a straight line. If the projectile were along a path for which the impact parameter is less than the radius $R$ of the target, there would be a collision between the two. On the other hand if the impact parameter were even slightly larger than $R$, the target wouldn't be in the path of the projectile and there would be no collision - the projectile would continue drifting past the target in a straight line.

If the projectile itself is a sphere with finite radius $r$, the situation would be slightly different. If we track the centre of the projectile and trace out its path, we would call the shortest distance between this path and the line parallel to it drawn through the centre of the target, the impact parameter. Then a collision would be inevitable if the impact parameter was less than the sum of the two radii ($r+R$). Whereas if the impact parameter was larger than this, the projectile would miss the target and there would be no collision. Therefore the impact parameter in such a case is determined by both the size of the target and that of the projectile. 

# Relation with scattering angle
In general when a projectile collides elastically with the target, the projectile gets deflected by some angle and the target recoils. For simplicity, let us assume the target is very massive and hence its recoil is negligible. The question we would like to answer is: how is the angle of deflection, also called the **scattering angle**, of the projectile related to the impact parameter? Obviously, the smaller the impact parameter, the larger is the scattering angle. But we'd like to obtain a precise mathematical relation between the two.

Let us denote the scattering angle by $\theta$. This is the angle between the straight line path of the projectile before the collision and its new deflected path after collision. Let $b$ be the impact parameter. Now, the projectile bounces off the target in such a way that the angle that the incident path makes with a line stretching through the centre of the sphere through the point of impact, equals the angle made by the deflected path with the same line through the centre. Let us call this angle $\alpha$.

From geometry it is evident that $b=R\sin\alpha$. Also, supplementarity requires that $\alpha+\alpha+\theta=180^o$ or $\alpha=90^o-{\theta\over2}$. Hence,

<div>
\begin{align*}
b&=R\sin\left(90^o-{\theta\over 2}\right)\\
b&=R\cos\left({\theta\over 2}\right)
\end{align*}
</div>

This is the relation between the impact parameter $b$ and the scattering angle $\theta$ that we were looking for. Let's test it. In case of a head-on collision, we have $\theta=180^o$. Then the impact parameter must be $b=R\cos(180)$. This means, $b=R\cos90^o=0$. Which was expected. $b=0$ means the path of the projectile coincides with the line connecting with the centre of the target, leading to a head-on collision.

On the other hand, if no collision must happen, the scattering angle is zero and we have, $b=R\cos0^o=R$. In fact, for any value $b\geq R$, the projectile misses the target and no deflection results. 

# When force fields are involved
Things get a little complicated when the target can apply force on the projectile even before they can get in contact. For example, when a proton is accelerated towards an atomic nucleus, we have the target and the projectile both positively charged and hence they repel one another. This repulsion is strongest in the vicinity of the target and becomes weak at large distances from it. So the proton, while it is at a large distance from the target, can be approximated to be a free particle, floating along a straight line. But as it nears the target nucleus, it's path curves away from it until it has gone far enough from the target where its path becomes a straight line again. The angle between the the incidence direction and the final deflected direction is the scattering angle here and can be measured readily through experimental detection of the scattered projectile.

The trick however is to ascertain the impact parameter. Recall that in order to measure the impact parameter, we ought to draw a line through the centre of the target parallel to the straight line path of the projectile. But the target is an atomic nucleus, which, before the collision happens, is as good as being invisible. Experiments with bubble chambers might reveal the tracks of the particles but cannot help us measure the impact parameter that is of the order of ${1\over 10,000,000}$ of a millimetre. In fact, when it comes to subatomic particles, the impact parameter is not a measurable entity. It can only be computed if the scattering angle is measured and a relation between $\theta$ and $b$ is known.

When collisions between celestial objects are considered, the measurement of the impact parameter is not an issue. However the attractive gravitational force tends to pull the projectiles inwards, hence yielding large values of the impact parameter that will lead to the projectile hitting the target. Moreover, such collisions are almost never elastic. If the projectile misses the target, we observe it deflect off its straight path but if the projectile does hit the target, we get nothing more than a crater and some dust.

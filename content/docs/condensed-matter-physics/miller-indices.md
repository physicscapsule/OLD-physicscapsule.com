---
title: "Miller Indices"
weight: 4
---

# Reference axes

Like with any three-dimensional object we use three reference axes to describe the geometry of a crystal. The choice of these axes is not always arbitrary; rather we choose axes with respect to key geometric properties of the crystal in question, which also means they vary by crystal. For example, for cubic crystals, we simply pick three mutually perpendicular axes, each parallel to one of three pairs of opposite faces on the cube. For a triclinic system picking three axes based on similar reasoning would give us three oblique axes, none of which form the familiar $ 90^\circ $angle. It is important to remember that mutual perpendicularity is not a norm---there is no need for it to be. It is far more important that the axes we choose represent the symmetry inherent in our crystal.

The purpose behind our choosing of reference axes is simple: if we were to know the mutual orientations of our three axes we should be able to plot points on our crystal. So long as we are consistent about our choice of reference axes for a given type of crystal replicating points universally becomes a trivial affair. This is exactly like plotting points relative to a three-dimensional Cartesian or Polar co-ordinate system.

# The right-hand screw

By convention crystallographic reference axes are labelled $ X \rightarrow Y \rightarrow Z $ in an anticlockwise direction when seen perpendicularly from above. If you can imagine tightening a traditional screw, this would be the direction in which the screw head would rotate if you looked at the screw from atop, along the direction in which it is moving forwards. As a result of this comparison we call the anticlockwise $ X \rightarrow Y \rightarrow Z $ orientation a \textbf{right-hand screw}.

We also define three interaxial angles formed between pairs of our reference axes. The one opposite $ X $, or between $ Y $ and $ Z $, is conventionally labelled $ \alpha $. Likewise the one opposite $ Y $ is called $ \beta $ and the one opposite $ Z $ is $ \gamma $. Keep in mind that these are just conventions and you are free to break them at the cost of ease of reading. Particularly in condensed matter physics this convention is followed rather strongly.

# Plotting points on crystals

Our aim now is to see how we can use our reference axes to describe, mathematically, planes, lines and points on crystals much like we would in regular three-dimensional space. Somewhat counterintuitively, we begin with planes and work up to points. Lines will be implicit once we are done with the other two and it would be redundant to discuss them separately. You will soon see this is in fact the easier approach when compared to starting with points and working down to planes.

## Planes

Think of a set of three reference axes as shown in the figure below. An arbitrary plane $ ABC $ can be drawn connecting points on the three axes. Let $ OA = a $, $ OB = b $, and $ OC = c $.

{{< figure src="/images/miller-indices.png" title="Reference axes set-up" caption="An arbitrary set of three reference axes along with a pair of crystallographic planes drawn on them." class="left" >}}

We know that to get to a point $ (X, Y, Z) $ on our plane we need to travel a length of $ X $ along the x-axis, a length of $ Y $ parallel to the Y-axis, and a length $Z$ in the z-direction.

If we drew a perpendicular from the origin to our plane (which is $ OG $ in the figure) we realise that a position vector to any point on the plane has a projection $ OG $. This is because any line joining a point on the plane to $ G $ will be perpendicular to $ OG $i.e. it will be a projection of the position vector of that point. In other words, the vector sum of $ X $, $ Y $ and $Z $ is a projection on OG. If these vectors form angles $ \chi $, $ \psi $ and $ \omega $ with respect to $ OG $ at the origin, their sum would be

<div>
$$
d = X \cos \chi + Y \cos \psi + Z \cos \omega
$$
</div>

where $ d $ is the length of $ OG $. But we can simplify this further. Consider triangle $ OAG $ for instance: since $ X $ lies on the same axis as $ OA $ it is clear that $ OA $ too forms an angle of $ \chi $ with $ OG $; likewise for $ OBG $ and $ OCG $. In other words

<div>
$$
d = a \cos \chi + b \cos \psi + c \cos \omega
$$
</div>

where we have used the fact that $ OA = a $, $ OB = b $ and $ OC = c $. We can now divide the two equations to arrive at the equation of a plane:

<div>
\begin{equation}
\boxed{ { X \over a } + { Y \over b } + { Z \over c } = 1 } \tag{1} \label{eq:plane}
\end{equation}
</div>

It is not hard to see that this equation applies to any plane that is oriented exactly like $ ABC $. That is to say, this equation represents an entire *family* of planes parallel to $ ABC $. Each plane arises by varying $ a $, $ b $ and $ c $ proportionately.

## Points

The idea of Miller indices arises from a description not of planes but of points. Specifically, returning to our figure above we realise that any plane may be described not by means of an equation but more simply with the help of three integer numbers which signify the points of intersection of that plane with the $ x $, $ y $ and $ z $ axes. We usually denote these intercepts by $ h $, $ k $ and $ l $ and call them **Miller indices** after the British scientist William Hallowes Miller who came up with this idea.

The reasoning for Miller indices is quite apparent once we define our approach. Say for some arbitrary plane $ ABC $ with intercepts at $ a $, $ b $ and $ c $ we set $ h = k = l = 1 $. Such a plane is simply denoted by $ (hkl) \equiv (111) $ and we call such a plane a **parametral plane**.

The benefit of using Miller indices becomes clearer when we consider any other plane of the same family, such as $ LMN $ marked in our figure, with Miller indices $ h $, $ k $ and $ l $ given as $ a/h $, $ b/h $ and $ c/h $ relative to the parametral plane with $ (hkl) \equiv (abc) $. Say the intercepts for $ LMN $ are some $ h = 3 $, $ k = 4 $ and $ l = 2 $. We can then represent the plane simply as $ (342) $.

Now what about the reverse? What if we described $ LMN $ as $ (hkl) \equiv (111) $ instead of $ ABC $? Once again, the beauty of the Miller indices lies in the fact that they are relative and it does not matter which plane we choose as our parametral plane so long as we get the family right. The indices of a family of planes $ ABC $ will still be related as $ a/h $, $ b/k $ and $ c/l$ but, unlike before we will end up with fractional values for our Miller indices. (We will discuss what this mean in the next section.)

Generally, what we have is $ a \rightarrow a/h $, $ b \rightarrow b/k $ and $ c \rightarrow c/l $ making eq. $ \eqref{eq:plane} $

<div>
\begin{equation}
\boxed{ { h X \over a } + { k Y \over b } + { l Z \over c } = 1 } \tag{2} \label{eq:miller}
\end{equation}
</div>

For a plane passing through the origin the right-hand side becomes zero since, at the origin, the plane must satisfy $ X = Y = Z = 0 $.

Points too are labelled the same way with position vectors going as $\mathbf{r} = h\mathbf{x} + k\mathbf{y} + l\mathbf{z} \equiv [hkl]$. Note the use of square brackets for Miller indices of points as opposed to parentheses for Miller indices of planes---this is another convention. In effect, $ [ \ldots ] $ denotes a direction in the crystal while $ ( \ldots ) $ denotes a set of planes. Further, to prevent redundancy, we use $ \langle \ldots \rangle $ to denote all planes that have the same symmetry as a $ ( \ldots ) $ family.

# The finer aspects

What we have discussed so far is a detailed look at Miller indices but our understanding of them will be incomplete if we do not make a few important observations. First, Miller indices refer to points of intersection along reference axes. They are relative which means we could try to cap them at $ 1 $ so that $ 0 < h, k, l < 1 $ but it is not hard to see why this will be futile: after all, parallel planes can extend to infinity. The alternative is to limit miller indices to integral values.

## Dealing with fractions

We saw above how we might end up with fractional Miller indices. Defining a parametral plane as $ (hkl) \equiv (111) $ might leave us with another plane that satisfies (as in the case of $ ABC $ above) something like $ 3a $, $ 6b $ and $ 2c $ giving us

<div>
$$
h = 1/3,\, k = 1/6 \textrm{ and } l = 1/2
$$
</div>

Rather than writing down our Miller indices for such a plane as fractions we adhere to our integers-only rule and multiply the entire set by its lowest common denominator. In this case we multiply by 6 to get

<div>
$$
ABC \equiv (2, 1, 3)
$$
</div>

## Dealing with negatives

It is perfectly alright for a plane or point to lie on one of the other quadrants where some of the axes are negative. In such cases the method of computing the Miller indices remains the same whereas the the index with a negative sign is denoted with a bar. So a point whose position is given by

<div>
$$
h = -{1\over 3} \quad k = -1 \quad l = {1\over 2}
$$
</div>

will have the Miller indices $ [\bar{2},\bar{6},3] $. Although not impossible, having a Miller index cross $ \pm 4 $ is quite rare.

## Dealing with planes parallel to axes

Finally, in our examples above the plane we chose, somewhat conveniently, always intercepted all three axes. But what if a plane never intercepts one or two of our axes? This can only happen if the plan is parallel to said axes because if it is not then the plane will intersect the axes at some point much like any two non-parallel lines. In such cases our Miller indices, derived from $ a/h,\,b/k,\,c/l$, will end up as, say, $ a/3,\,b,\,(\infty) c $. That is to say, the plane will intercept the $ z $-axis at infinity or...never. In such cases the index $ l = 1/\infty = 0 $ and our three Miller indices would be 1, 3 and 0.

Lastly, keep in mind that a plane parallel to one of our axes will necessarily have four corners since a crystallographic plane has to extend infinitely. Further, as we discussed earlier, Miller indices, whether for points or planes, are relative because they have to satisfy a crystal structure that is repetitive and, with respect to an arbitrary origin, isomorphic. So, given a set of Miller indices, regardless of your choice of origin you will describe relatively the same family of planes or the same point relative to the origin, thereby making it easy to do further mathematics based on these helpful indices.

---
title: "Classical vs Quantum States"
date: 2019-04-13T22:00:01+05:30
---

Imagine a hunter quietly sneaking through the bushes in a forest, positions himself carefully and points his loaded rifle straight at a rabbit he just spotted. The rabbit seems to have sensed the imminent threat and stands still with his ears up. Once the hunter pulls the trigger, there's very little time between the bullet leaving the rifle and hitting the rabbit (assuming the aim was good). However short the time, the bullet does take a path in reaching the rabbit. If we slow down time right when the trigger was pulled and observe the bullet leaving the rifle, the question we ask is how can we calculate whether or not the bullet will hit the rabbit. In other words, how can we predict what path the bullet will take. If the path coincides with the still position of the rabbit, we'll know that the bullet did hit the rabbit. 

# Trajectories

To make our analysis rigorous, we think in terms of where the bullet is and how fast it's moving, at different instants of time. Clearly, just before the bullet was fired, its position was inside the rifle muzzle and its speed was zero. But after the firing, the bullet moved to positions outside the rifle and had a large speed in the direction of the rabbit. Until the bullet reached the rabbit, we can imagine a series of positions marked all along its path, each of which is linked with the speed that the bullet had when it was there. These series of positions is what we call the **trajectory** of the bullet. Velocity is crucial for our understanding of the trajectory because where the next position of the bullet will be at the next instant of time depends on how fast the bullet was travelling at the previous instant and in what direction. 

# The classical state

Such pairs of numbers - position and velocity - are all that we need to know the subsequent motion of the bullet. We attach central importance to such pairs and call each of them the **state** of the bullet. Therefore, at any instant of time during its flight, the bullet's state would be mentioned by specifying its position and velocity at that instant. Even if the velocity of the bullet doesn't change at all, the change in the position of the bullet would lead us to say that the state of the bullet has changed. On the other hand, during all the time that the bullet rested inside the rifle, we'd say the state of the bullet remained the same (with respect to the rifle), since neither its position nor its velocity changed then.

The same is true of any other classical system (classical meaning here relating to the description given by Newton). The state of the system is simply the information about the positions and the velocities of its constituent particles. By system we could mean the single bullet fired from a rifle, or a billiard ball rolling on a table or even a gas filled in a sealed box (imagined to be made of a large number of molecules) or a pendulum attached to a ceiling, swinging gently.

# Tracking the trajectories

As we saw earlier, the series of positions and corresponding velocities of any object decides what the trajectory of the particle is. The trajectory could surely be affected by external forces on the object. In the case of the bullet, the moment it left the rifle, it wasn't free from any forces, gravity still acted on it, pulling it down very slightly. And so the trajectory of the bullet wouldn't be strictly a straight line but a curved one (however slightly) towards the ground. To account for this, we make use of Newton's laws of motion that give a nice connection between the position of any object and the forces experienced by it.

To put it mathematically, the pair of numbers $(\vec{r},\vec{v})$ characterises the state of the system at any instant of time. In general, both the position and velcoity could be functions of time, $\left(\vec{r}(t), \vec{v}(t)\right)$. Now, say we know the position and velcoity of the object at one instant of time. Let us call this instant $t=0$. This is when we reset our stop clocks. Let's call these initial values of position and velocity, $\vec{r}(0)=\vec{r}_0$ and $\vec{v}(0)=\vec{v}_0$. Newton's second law allows us to write the relation, \[\vec{F}=m\vec{a}\] assuming the mass of the object doesn't change as it moves under the influcence of the force $\vec{F}$. Here $\vec{a}$ is the acceleration of the object, telling us how quickly its velocity is changing (if at all it is), $\vec{a}={\mathrm{d}\vec{v}\over\mathrm{d}t}$. We therefore, have
\[\mathrm{d}\vec{v}=\vec{a}\,\mathrm{d}t\]
What this equation tells us is how much does the velocity of the obejct change during a time time interval $\mathrm{d}t$. Intergating this equation will give us the total change in the velocity of the object during a finite time interval between $0$ and $t$.

<div>
\begin{align*}
\int_{v_0}^v\mathrm{d}\vec{v}&=\int_0^t\vec{a}\,\mathrm{d}t\\
\vec{v}-\vec{v}_0&=\vec{a}t\\
\vec{v}&=\vec{v}_0+\vec{a}t
\end{align*}
</div>

But then the velocity itself is defiend as the rate of change of position, $\vec{v}={\mathrm{d}\vec{r}\over\mathrm{d}t}$. Hence,

<div>
\begin{align*}
{\mathrm{d}\vec{r}\over\mathrm{d}t}&=\vec{v}_0+\vec{a}t\\
\mathrm{d}\vec{r}&=(\vec{v}_0+\vec{a}t)\mathrm{d}t
\end{align*}
</div>
 
Integrating as before,

<div> 
\begin{align*}
 \int_{r_0}^r\mathrm{d}\vec{r}&=\int_0^t(\vec{v}_0+\vec{a}t)\mathrm{d}t\\
 \vec{r}-\vec{r}_0&=\vec{v}_0t+{1\over 2}\vec{a}t^2\\
 \vec{r}(t)&=\vec{r}_0+\vec{v}_0t+{1\over 2}\vec{a}t^2
 \end{align*}
</div>
 
 This last equation is the penultimate aim of Newtonian mechanics. Knowing where a particle was ($\vec{r}_0$) and how fast and in what direction it moved ($\vec{v}_0$), at some initial instant ($t=0$), and knowing what its acceleration is ($\vec{a}={\vec{F}\over m}$),we can calculate the position $\vec{r}(t)$ of the obejct at any later time $t$.

With regard to the hunter's fired bullet, if we knew with what velocity it left the rifle and what was the location of the rifle (and of the bullet inside it) then we could compute the subsequent positions of the bullet at any later instants of time, allowing us to trace the bullet's path (it's trajectory). In the language that we've used, if at any instant of time $t$, the position $\vec{r}(t)$ was also the position of the rabbit (assumed to be stationary), the hunter would have made the kill successfully.

# A strange condition

Now that you have a fair understanding of what the meaning of the state of a system is in Newtonian mechanics and how any object's trajectory can be calculated, let us think of a possibility of describing the motion of the object if just one thing was different: if you could not ascertain the values of the position and the velocity of the object at the same time and were allowed to know only one at a time, how would you go about describing the motion of the object? We're not just speaking of a delay in knowing but a limit of knowing itself. At any given instant of time, you have to make a choice whether you want to know the object's position or its velocity. You could never know both of these at the same instant of time. Where would you start describing the motion?

This would also mean you could not know the initial position and velcoity both, since they were measured at the same instant ($t=0$). And most significantly, what meaning would be left for the trajectory of an object? Recall that the trajectory is simply the path taken by the obejct and is built by marking the positions of the object at different instants of time. In order to mark the next point of the trajectory, we need to know where was the previous position of the obejct as well as what its velocity was then. If say we ascertained the previous position but know nothing of what its velocity was then, how do we know in what direction the object moved? And where at all would we decide to mark the next point of the trajectory?

# A new way of thinking

Well, if we cannot know both the position and velocity of the obejct at the same time, why don't we measure its velocity and just "see" the position of the particle. But then isn't seeing, knowing? The condition we imposed was not that you cannot see both the position and velocity at the same time but that you cnanot know them at all. We hope you've arrived at a situation where you think we simply cannot proceed in determining the motion of the particle and continue using the old defition of the state of the object as the values of its position and velocity at the given instant of time. We either must ward off the superficial condition, since it's just our imagination, or we must find a radical way of thinking about the situation. The former view may be accepted if we are considering regular obejcts at least big enough to be seen by a normal naked eye. But it turns out that such a bizarre condition on knowing the position and velocity of an object at the same time is actually a rule of nature when we study microscopic objects.

As strange as it might sound, this is the truth when we go down to the scale of molecules and atoms. For mysterious reasons, we cannot know both the position and velocity of the particles, goverend by the famous Heisenberg uncertainty principle. Therefore, we are left with no choice but to think of a very radical way of describing the phenomena of the atomic world. In contrast to Newtonian mechanics, we call this new adventure, quantum mechanics. 

# The quantum state

In deciding to proceed any farther, we must also make up our minds to let go of many of our common sense notions. As we already saw, the very concept of the path taken by an obejct becomes meaningless under the new conditions. This is something we have never come across in Newtonian mechanics that described bigger objects that could be seen with our bare eyes. No matter whether or not we could measure or calculate the objects trajectories, we always had the luxury of being able to see the paths taken by moving objects. But this isn't the case with microscopic objects. We no longer can see things with our eyes. All we can do is meausre indirectly and use logic, sometimes unconventional one, to arrive at ``sensible'' results. 
 
This radical way of thinking begins with abandoning the old defintion of the state of a system. We no longer have the convenience of knowing both the position and the velocity of objects to even begin speaking of the state of the system. We need to redefine what we mean by the state of a quantum system. 
 
# Using what we know
 
Even though we aren't anymore allowed to use the exact same methods that Newton used, we can at least seek guidance in terms of the structure of thought regarding how to go about defining things. 
 
Recall that Newton's methods allowed us to calculate the state of the system at any instant of time if we knew its state at one specific time (which we called the initial instant, $t=0$). We would expect the new quantum state to behave in a similar manner - knowing the state of the system at one instant should allow us to calculate its state at any other time. 
 
Also knowing the state of the system at one instant of time, allowed us to obtain the trajectory $\vec{r}(t)$ of the system. And this knowledge of the position as a function of time must allow use to compute a numbe rof other quantities associated with the system and its motion. For example, once the position $\vec{r}(t)$ is known as a function of time, all we ought to do to know how fast the particle was moving and in what direction, at any other time $t$, is to differentiate it, ${\mathrm{d}\vec{r}(t)\over \mathrm{d}t}=\vec{v}(t)$. Knwoing the velocity must allow for the computation of its momentum, $\vec{p}(t)=m\vec{v}$. Simiarly, through a series of well-defined mathematical operations we can determine the objects acceleration, angular momentum, force, torque, etc. However without the knowldege of the trjaectory, or one step back, the state of the system, we could never know anything about its motion.
 
We would therefore like our quantum state to behave similarly - knowing the state is tantamount to knowing everything there is to know about the system. How we go about doing this will not of course be the same as we did in Newtonian mechanics. For if we did so, we are not on the path of a radical way of thinking about the situation but are merely calling the state of the system, the quantum state of the system. We aren't just fond of tacking on the word ``quantum'' before the already familiar quantities and call it a new way of thinking. This, you may also realise, if you actually proceeded so. You'll soon come across the concept of position and velocity of the system and again be restricted to know only one of them by the uncertainty principle. We'd be caught in a miserable loop then. 
 
# The definition
 
Since we certainly can't work backwards by first observing the objects and then coming up with a description, in case of quantum systems, we have to build our understanding by defining what the new quantum state is.  In the simplest of words, we define the quantum state of a system to be a function of space and time, usually denoted by $\psi(\vec{r},t)$, (here $\psi$ is a greek alphabet, pronounced "psi") that contains all the information about the system that can be meaningfully retrieved. The reason we expect the quantum state to be a function of space and time is again in analogy with the classical state. Recall that the classical state was specified by the pair $(\vec{r}(t), \vec{v}(t))$ or, since velocity is derived from position, $\left(\vec{r}(t),{\mathrm{d}\vec{r}(t)\over\mathrm{d}t}\right)$. Therefore there is an ultimate dependence of the state of a system at any instant of time on its position at that instant. In short, even the classical state is a function of space and time. But be sure of the fact that we do not as yet know what the dependence is. We just expect it to exist.

Also note that so far we aren't clear as to how the above said retrieving of meaningful information from the quantum state can be done but we simply have faith that it can be done. With this faith, we have begun one of the strangest journeys that the human mind has ever set out on in the quest of understanding nature at possibly its deepest level.

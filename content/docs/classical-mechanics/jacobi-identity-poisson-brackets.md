---
title: "Jacobi Identity Poisson Brackets"
date: 2019-04-13T10:49:33+05:30
---

We said in our discussions of Poisson brackets in (chapter: Poisson brackets) that there exists what is called (index: Jacobi?s identity)?see (eq: eqjacobi-identity chapter: Poisson brackets num: 7). We shall attempt to prove this relation in this chapter. Although such well-known books as Herbert Goldstein?s claim that Jacobi?s identity is somewhat hard to prove without rigorous algebra we doubt this is true.

Further, there is no need to employ custom notations as (some physicists target:\_blank)[http://cds.cern.ch/record/587483/files/0210074.pdf] have done. In this chapter the only shorthand we shall use is the standard $\\partial\_x y$ notation in reference to the lengthier $\\partial y / \\partial x$ for its simplicity. And, before we begin, recall that a Poisson bracket between $f(q,p)$ and $g(q,p)$ is defined as $[f,g] = \\partial\_qf\\partial\_pg-\\partial\_pf\\partial\_qg$.

- - - - - -

## **Statement:**
 *Jacobi?s identity is given by the relation*

$$ \\begin{equation} [f,[g,h]] + [g,[h,f]] + [h,[f,g]] = 0 \\label{eq:jacobi-identity} \\end{equation} $$

# **Proof:** 
We can write the time-variation of $\\varphi(q,p)$ as $$\\begin{align\*}{\\textrm{d}\\varphi\\over\\textrm{d}t} &= \\partial\_q\\varphi\\textrm{d} ot{q} + \\partial\_p\\varphi\\textrm{d} ot{p} \\\\[.5em] &= \\partial\_q\\varphi\\partial\_pH - \\partial\_p\\varphi\\partial\_qH \\\\[.5em] &= [\\varphi,H]\\end{align\*}$$

where we have used Hamilton?s (index: Canonical equations) discussed in (chapter: Hamilton's canonical equations) which tell us that $\\textrm{d} ot{q} = \\partial\_pH$ and $\\textrm{d} ot{p} = - \\partial\_qH$ for the Hamiltonian $H$ of some system.

In all these cases, keep in mind, our (index: Generalised coördinates) and (index: Generalised momenta) are $n$ in number, which means all our $q$ and $p$ are essentially $q\_i$ and $p\_i$ and summed over all $n$. The subscripts are assumed to be implied and are omitted here for simplicity.

We now take the time derivative of the Poisson bracket of $f$ and $g$ to get $${\\textrm{d} \\over\\textrm{d}  t}[f,g] = \\left[ {\\textrm{d}  f\\over \\textrm{d}  t},g\\right] + \\left[f,{\\textrm{d}  g\\over \\textrm{d}  t}\\right]$$where the time derivatives?including the entire left-hand side?are know, from our result above, to be Poisson brackets themselves. Therefore, $$[[f,g],H] = [[f,H],g] + [f,[g,H]]$$

A simple application[^ Note that we apply the property twice to the $f$, $H$, $g$ term; we do so once to each bracket and end up with the second term in eq. $\\eqref{eq:jacobi-identity}$.] of the antisymmetry property of Poisson brackets ((eq:eqantisymmetry chapter: Poisson brackets num: 3)) gives us Jacobi?s identity: $$[f,[g,H]] + [g,[H,f]] + [H,[f,g]] \\tag{\\ref{eq:jacobi-identity}}$$

- - - - - -

# Further

One might argue with the proof above saying it applies exclusively when one of the three functions is the Hamiltonian. This is not the case and we can readily show that the same procedure works for any generating function $h$?a choice of notation, and nothing more, that keeps us in line with eq. $\\eqref{eq:jacobi-identity}$.

Consider the definition of a Poisson bracket being acted upon by an infinitesimal (index: Canonical transformation) $\\textrm{d} elta$. We know that $$\\begin{align\*}\\textrm{d} elta [f,g] &= \\epsilon [[f,g],h]\\\\[.5em] [\\textrm{d} elta f,g] + [f,\\textrm{d} elta g] &= \\epsilon [[f,g],h] \\\\[.5em] \\epsilon [[f,h],g] + \\epsilon [f,[g,h]] &= \\epsilon [[f,g],h] \\end{align\*}$$where $h$ is our generating function that has the property $\\textrm{d} elta \\varphi = \\epsilon [\\varphi, h]$ and $\\epsilon$ is an appropriate scalar correction term. We make use of the linearity of Poisson brackets ((eq:eqlinearity chapter: Poisson brackets num: 5)) while handling $\\epsilon$. On rearranging this equation exactly as we did above we end up with eq. $\\eqref{eq:jacobi-identity}$.

In the above set of steps the left-hand side tells us that the application of $\\textrm{d} elta$ only relies on variations in $f$ and $g$ and not, at least directly, on the generalised variables $p$ and $q$ on which they depend.

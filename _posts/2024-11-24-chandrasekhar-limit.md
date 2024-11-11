---
layout: post
title:  Chandrasekhar Limit
description: Dare to dream?
date:   2024-11-10 15:01:35 +0300
image:  '/images/chandrasekharlimit.png'
tags:   [Physics]
---

### A Life in the Service of Science

Subrahmanyan Chandrasekhar, an astrophysicist renowned for his transformative contributions to our understanding of stellar evolution and black holes, was as remarkable for his humility as he was for his genius. A Nobel laureate best known for discovering the “Chandrasekhar limit,” his life was shaped by an unyielding pursuit of knowledge, a meticulous work ethic, and a unique approach to learning. Rather than seeking fame, Chandrasekhar sought mastery. He would exhaustively explore a field, produce seminal work, then move on to the next scientific challenge, leaving behind an impressive array of discoveries across astrophysics.

His commitment to science was legendary. In one famous example, Chandrasekhar traveled from Yerkes Observatory in Wisconsin to the University of Chicago every week, a round trip of nearly 80 kilometers, to teach a course attended by just two students. When asked why he would undertake such an effort for so few, Chandrasekhar simply replied, “They are very good students.” This response epitomizes his devotion to scholarship, seeing each interaction with students as an opportunity to share and deepen understanding. 

Chandrasekhar’s scientific philosophy was one of relentless exploration, driven by curiosity rather than the pursuit of conclusions. This mindset is evident in his unique approach to research. Throughout his career, Chandrasekhar chose to concentrate on specific topics exhaustively. He would delve into one area, produce groundbreaking insights, publish several influential papers, and then move on to the next field. Over the decades, this pattern allowed him to make significant contributions across various areas in physics, from stellar dynamics and black holes to radiative transfer and fluid dynamics.

### Discovering the Chandrasekhar Limit

Chandrasekhar’s most celebrated achievement, the discovery of the Chandrasekhar limit, revolutionized astrophysics by establishing the maximum mass that a white dwarf star can sustain before collapsing into a denser state, ultimately forming a neutron star or black hole. This insight laid the foundation for understanding stellar life cycles and revealed the fates awaiting stars of varying masses. Yet, the discovery was not easily accepted; the idea of black holes was still considered controversial, and prominent scientists, including Sir Arthur Eddington, initially resisted his findings.

However, Chandrasekhar’s perseverance never wavered. Guided by a belief that “the simple joy of exploring the mind” was worth any hardship, he held fast to his calculations and allowed time to prove their validity. In the years that followed, his theories gained widespread acceptance, profoundly influencing our understanding of the universe and securing his place as a pioneer in astrophysics.


<script type="text/javascript">
MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']],
    displayMath: [['$$', '$$'], ['\\[', '\\]']]
  }
};
</script>
<script type="text/javascript" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

# Derivation of the Chandrasekhar Limit

The Chandrasekhar limit represents the maximum mass $\textcolor{turquoise}{M}$ that a white dwarf star can possess before gravitational collapse overcomes electron degeneracy pressure, leading to a neutron star or black hole. This derivation combines principles of quantum mechanics and general relativity to establish a limit around 1.4 solar masses. Here's the breakdown for the common variables in this derivation:


## Variables and Constants

1. **Total Mass** $\textcolor{turquoise}{M}$: The total mass of the white dwarf.
2. **Radius** $\textcolor{turquoise}{R}$: The radius of the white dwarf, influenced by the mass-density relation.
3. **Density** $\textcolor{turquoise}{\rho}$: Defined as $\textcolor{turquoise}{ \rho = \frac{M}{\frac{4}{3} \pi R^3} }$, representing the star's density.
4. **Electron Mass** $\textcolor{turquoise}{m_e}$: Mass of an electron, crucial in determining the degeneracy pressure.
5. **Proton Mass** $\textcolor{turquoise}{m_p}$: Mass of a proton, relating to the hydrogen composition and the electron-proton ratio.
6. **Planck's Constant** $\textcolor{turquoise}{h}$: A quantum mechanical constant essential in calculating momentum.
7. **Speed of Light** $\textcolor{turquoise}{c}$: The speed of light, included for relativistic considerations.
8. **Gravitational Constant** $\textcolor{turquoise}{G}$: Governs the gravitational force trying to collapse the star.

## Step-by-Step Derivation

### Step 1: Defining Degeneracy Pressure

The pressure exerted by a gas of relativistic electrons, or **degeneracy pressure** $\textcolor{turquoise}{P}$, is given by the Fermi momentum $\textcolor{turquoise}{p_F}$. For an electron gas, the Fermi momentum can be defined as:

<p style="color:turquoise" align="center"> 
$$
p_F = \textcolor{turquoise}{\left(3 \pi^2 \frac{Z}{A} \frac{\rho}{m_p} \right)^{\frac{1}{3}} h}
$$
</p>

where $\textcolor{turquoise}{Z}$ is the atomic number, $\textcolor{turquoise}{A}$ is the mass number, and $\textcolor{turquoise}{m_p}$ is the proton mass. The degeneracy pressure for relativistic electrons is then:

<p style="color:turquoise" align="center"> 
$$
P \approx \textcolor{turquoise}{\frac{p_F c}{3} \left(\frac{p_F}{m_e c} \right)^3}
$$
</p>

### Step 2: Balancing Forces

In a stable white dwarf, the **gravitational pressure** $\textcolor{turquoise}{P_{\text{gravity}}}$ is balanced by the electron degeneracy pressure $\textcolor{turquoise}{P}$.

The gravitational pressure is given by:

<p style="color:turquoise" align="center"> 
$$
P_{\text{gravity}} \approx \textcolor{turquoise}{\frac{G M^2}{R^4}}
$$
</p>

### Step 3: Expressing Mass in Terms of Radius

To balance gravitational pressure with degeneracy pressure, equate $\textcolor{turquoise}{P_{\text{gravity}}}$ with $\textcolor{turquoise}{P}$:

<p style="color:turquoise" align="center"> 
$$
\frac{G M^2}{R^4} = \textcolor{turquoise}{\frac{p_F c}{3} \left(\frac{p_F}{m_e c} \right)^3}
$$
</p>

This relationship implies that as mass $\textcolor{turquoise}{M}$ increases, so must the density $\textcolor{turquoise}{\rho}$, which in turn raises the Fermi momentum $\textcolor{turquoise}{p_F}$ until electrons reach relativistic speeds. 

### Step 4: Deriving the Mass Limit

Rearrange and simplify the expression above to solve for $\textcolor{turquoise}{M}$ in terms of constants. After balancing these terms, we find that:

<p style="color:turquoise" align="center"> 
$$
M_{\text{Ch}} \approx \textcolor{turquoise}{1.4 M_{\odot}}
$$
</p>

where $\textcolor{turquoise}{M_{\odot}}$ is the mass of the Sun. This value represents the Chandrasekhar limit—the maximum mass a white dwarf can have before electron degeneracy pressure fails to counteract gravity, leading to a collapse.

## Summary of the Chandrasekhar Limit

The Chandrasekhar limit represents the tipping point at which electron degeneracy pressure can no longer counterbalance gravitational collapse in a white dwarf star. Beyond this limit, the star undergoes a dramatic transformation, potentially collapsing into a neutron star or even a black hole. This fundamental astrophysical concept explains the behavior and ultimate fate of stars at the end of their life cycles, laying the groundwork for modern studies of stellar evolution and compact objects.


#### A Lifetime of Achievement Across Fields: "Success is Not a Destination, But the Road That You’re On"

Chandrasekhar’s intellectual curiosity and commitment to science extended across multiple disciplines within physics, each with equal dedication and depth. After he had published extensively on one topic, he would immerse himself in a completely different area, challenging himself anew and continuing to push the boundaries of his understanding. His contributions included foundational research on radiative transfer, the theory of black holes, fluid dynamics, and general relativity. Each venture into a new field was marked by an intense, focused exploration that typically resulted in pioneering papers and books. 
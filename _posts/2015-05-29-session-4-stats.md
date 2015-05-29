---
layout: post
title: Statistical Characterization
description:
tags: [ERES, Stat Characterization]
image:
  feature: banner.jpg
  credit: ESO, Nathaniel C. Sheetz
  creditlink: 
---
Our post-lunch session is chaired by recent PSU PhD, Dr. Benjamin Nelson. These talks are all related to characterization of exoplanet systems using statistical methods.

---
***Systematics-insensitive periodic signal search with K2* (Ruth Angus, University of Oxford)**

When the second reaction wheel of *Kepler* failed, it was recommissioned as the K2 mission. The issue with the K2 mission is that the telescope itself drifts slowly, and they need to fire the thrusters every so often to fix this issue. That mean that, as the star appear to be drifting across the CCD, the precision of K2 has decreased compared to its predecessor.

To compensate for this, they need to come up with a better analysis algorithm for the K2 lightcurves. This involves better modeling of the stellar systematics and convolving that with a sine wave over many many frequencies to create a systematics insensitive periodogram (SIP). The raw periodogram of K2 data shows a very large feature at the 6 hour thruster times along with aliases of that 6 hour frequency. When they redo the lightcurve periodogram with SIP they are able to remove that large systematic feature and pull out the red giant acoustic oscillations of the host stars.

Using SIP, you can also find a better estimation of the stellar rotation period, since the systematics won't be clogging up the periodogram anymore. They were able to accurately recover the stellar rotation period once the systematics were removed from the lightcurves using SIP. They can also use this method to find other periodic signals like short period exoplanets, RR Lyrae, and eclipsing binary stars. Their code is available on [GitHub](https://github.com/RuthAngus/SIPK2) (don't use the tweated version!), and the paper recently came out on the [arXiv](http://arxiv.org/abs/1505.07105).


---
***A Catalog of Transit Timing Posterior Distributions for all Kepler Planet Candidate Events* (Benjamin Montet, Caltech/Harvard)**

Ben is working on a number of projects, including a transiting brown dwarf LHS-6343 and a paper on young M-dwarfs. Today he is talking about  transit timing variations (TTVs) (which Daniel Jontof-Hutter talked about yesterday). TTVs can ell us about eccentricities, inclinations, and mass ratios of planets in the same system, all of which can be really difficult to measure using another method.

When looking at TTV curves, the variations in transit timing usually follow a sinusoid, but not all points follow this trend. The current methods ignore non-Gaussian errors, assume white noise, ignore ill-fitting transits, short cadence data, and don't marginalize over transit shape (if the transit is not properly sampled, current methods usually ignore these points). But correlated noise matters too, and needs to be included in analyses.

Posteriors can help with this. If you fit many transit model models and times of transits, infer the posterior distribution for the time of every transit observed with *Kepler*, you can use importance sampling to get a handle on correlated noise. Importance sampling can help speed up your computation process bu focusing your computation on places in your data that you know, a priori, that the transits will be occurring. They are currently working on all of the single-transit systems, and multiple systems are nearly ready for "prime time". They are also looking for a cool name for the project, so give him a shout if you have an idea.


---
***Towards a Galactic Distribution of Exoplanets* (Matthew Penny)**


---
***Constraining the Demographics of Exoplanets Using Results from Multiple Detection Methods* (Christian Clanton)**


---
***Sifting Through the Noise - Recalculating the Frequency of Earth-Sized Planets Around Kepler-Stars* (Ari Silburt)**


---
***A population-based Habitable Zone perspective* (Andras Zsom)**


---
The session following the coffee break will be co-chaired by me (Kimberly), so that blog post will be written by Robert again.
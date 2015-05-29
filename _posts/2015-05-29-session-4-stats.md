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

Using SIP, you can also find a better estimation of the stellar rotation period, since the systematics won't be clogging up the periodogram anymore. They were able to accurately recover the stellar rotation period once the systematics were removed from the lightcurves using SIP. They can also use this method to find other periodic signals like short period exoplanets, RR Lyrae, and eclipsing binary stars. Their code is available on GitHub (don't use the tweated version!), and the paper recently came out on the arXiv.


---
***A Catalog of Transit Timing Posterior Distributions for all Kepler Planet Candidate Events* (Benjamin Montet)**


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
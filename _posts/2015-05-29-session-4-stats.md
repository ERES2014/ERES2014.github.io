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

<iframe width="560" height="315" src="https://www.youtube.com/embed/AuUleI68dwE" frameborder="0" allowfullscreen></iframe>

---
***A Catalog of Transit Timing Posterior Distributions for all Kepler Planet Candidate Events* (Benjamin Montet, Caltech/Harvard)**

Ben is working on a number of projects, including a transiting brown dwarf LHS-6343 and a paper on young M-dwarfs. Today he is talking about  transit timing variations (TTVs) (which Daniel Jontof-Hutter talked about yesterday). TTVs can ell us about eccentricities, inclinations, and mass ratios of planets in the same system, all of which can be really difficult to measure using another method.

When looking at TTV curves, the variations in transit timing usually follow a sinusoid, but not all points follow this trend. The current methods ignore non-Gaussian errors, assume white noise, ignore ill-fitting transits, short cadence data, and don't marginalize over transit shape (if the transit is not properly sampled, current methods usually ignore these points). But correlated noise matters too, and needs to be included in analyses.

Posteriors can help with this. If you fit many transit model models and times of transits, infer the posterior distribution for the time of every transit observed with *Kepler*, you can use importance sampling to get a handle on correlated noise. Importance sampling can help speed up your computation process bu focusing your computation on places in your data that you know, a priori, that the transits will be occurring. They are currently working on all of the single-transit systems, and multiple systems are nearly ready for "prime time". They are also looking for a cool name for the project, so give him a shout if you have an idea.

<iframe width="560" height="315" src="https://www.youtube.com/embed/SFLky-4uWIo" frameborder="0" allowfullscreen></iframe>

---
***Towards a Galactic Distribution of Exoplanets* (Matthew Penny, Ohio State University)**

Where are the known exoplanets? Microlensing is the only technique we currently have for probing for exoplanets in multiple areas of the galaxy. RV surveys are limited to nearby stars, *Kepler* looked in one region, K2 will add a ring around the solar system with more nearby targets, but microlensing surveys look straight into the galactic center to find the frequency of exoplanets as a function of galactic radial position.

Question: does plane formation in the bulge differ from the disk of the galaxy? Different galactic environments can have detrimental effects on the longevity of a protoplanetary disk, or can change the temperature of the protoplanetary disk to impede planet formation. They find that, based on microlensing surveys, there are a lot fewer planets in the galactic bulge than in the disk. They determine this by varying the ratio of disk planet formation efficiency to bulge planet formation efficiency to model the current distance distribution of microlensing planets. They find in their first results that the bulge planet formation efficiency must be lower than the disk planet formation efficiency in order to approximate the microlensing planet distance distribution that they see.

They want to find out what is the most probable distance/location in the galaxy to find exoplanets. They can measure distances to microlensing planets with parallax (for nearby planets), using a Bayesian method, or using the relative proper motions of stars to calculate the distances. While there are still some kinks to work out, this mix of techniques lets them probe a wide range of planet distances and begin to map the galactic distribution of exoplanets.



---
***Constraining the Demographics of Exoplanets Using Results from Multiple Detection Methods* (Christian Clanton, Ohio State University)**

There have so far been about 150 confirmed exoplanets around M-dwarf stars. Confirming these planets really takes a collaborative effort between multiple detection methods. M-dwarfs are good targets for exoplanets because they are the most numerous of stars in the galaxy, RV and microlensing surveys are also more sensitive to lower-mass stars.

There have been individual exoplanet censuses of M-dwarfs using separate methods. Some constrain the actual frequency of planets around these stars, other non-detections (direct imaging) place upper limits on this number. If they combine the results from these various techniques (microlensing + RV, and now direct imaging), they can confirm quite a few planets around M-dwarfs and get a constrain on long-period giant planets around these stars. They ask: is there a single planet population distribution that is consistent with all of these M-dwarf exoplanet surveys?

They map the distribution of planets into distributions of the observables relevant to each technique (microlensing+RV+direct imaging). They then determine the number of expected detections for each survey, and compare that with the actual reported results and determine a likelihood of that particular planet population, and repeat for a variety of planet populations. They can then constrain the planetary mass function and power law slope of this distribution very well for M-dwarfs. What this means is that the results of the microlensing, RV, and direct imaging surveys are consistent with a single planet population distribution. They also want to include the results from *Kepler* to add constraints from transit surveys as well.

<iframe width="560" height="315" src="https://www.youtube.com/embed/WZfowIuok8g" frameborder="0" allowfullscreen></iframe>

---
***Sifting Through the Noise - Recalculating the Frequency of Earth-Sized Planets Around Kepler-Stars* (Ari Silburt, University of Toronto)**

*Kepler* has been invaluable in attempting to answer the age-old question of: is our planet unique? Unfortunately, we haven't yet found a true Earth-analog. We can estimate the frequency of Earth-like planet by extrapolating our results past our detection biases. We first have to overcome our geometric bias: only certain planetary systems are transiting, and there's a large population of planets that we simply don't see in transiting surveys because of this detection bias. This is a strong function of planetary radius and orbital semi-major axis. 

This bias causes a lot of large error bars and false-positives in the *Kepler* data - mainly because we don't understand the stars themselves. Such large error bars can skew our estimation of the number and frequency of Earth-sized planets. What they've done is a new way of accounting for the uncertainty in planetary radius by applying our known *Kepler* detection probabilities for planets based on their radii and combining that with the probability curve of the planet size. For example, the uncertainties of a detection may include a very small size, but we know that detecting something that small is very unlikely, so that value is downweighted. This allows them to correct our error distribution and use this to improve our estimate of the frequency of Earth-sized planets.

They find that with these corrections, the frequency of Earth-sized planets in the *Kepler* sample is eta_Earth = 6.4%, which is about half of what it would be if they haven't accounted for the detection biases of *Kepler*. They anticipate that the Gaia spacecraft will help better understand the stellar exoplanet hosts, which will further increase the accuracy of their eta-Earth value.

<iframe width="560" height="315" src="https://www.youtube.com/embed/t1RfwmlSy7A" frameborder="0" allowfullscreen></iframe>

---
***A population-based Habitable Zone perspective* (Andras Zsom, MIT)**

Most people visualize a habitable zone as a stripe around a star that is capable of supporting liquid water. If you look at it in a population perspective, you can see which planets fall interior to the HZ and are covered in water vapor, those exterior to the HZ with ice on their surface (or like Mars that falls right on the ice/vapor limit), and those inside the HZ which can have liquid water.

From observations we have good estimates on the stellar properties and planetary orbital properties, but we don't know much about the planet properties and surface climate. How can we know the surface climate without knowing the planetary atmosphere?  They describe the HZ as a probability function to estimate the occurrence rate of HZ planets based on this HZ probability. If you treat the stellar and planet properties as random variables, you can create probability density functions out of them. They then sample each variable and use a 1D climate model to calculate the surface climate, repeat this to create an ensemble of climates, and then study the habitable sub-population and calculate their probabilistic HZ.

They find that the most probable area of HZ planets around M-dwarfs occurs around a few times the radius of the Earth, and around 0.5-1 times the stellar flux received at Earth (author's note: this is a really cool 2D HZ probability plot!). So, they find that the occurrence rate of HZ planets is 0.001-0.3 planet/star for M-dwarfs, but that the surface pressure and atmosphere type strongly impact the surface climate and occurrence rate. We need better estimate of the potential atmospheres of exoplanets. Their code is called HUNTER and is available on [GitHub](https://github.com/andraszsom/HUNTER).

<iframe width="560" height="315" src="https://www.youtube.com/embed/25hHDj84tnM" frameborder="0" allowfullscreen></iframe>

---
The session following the coffee break will be co-chaired by me (Kimberly), so that blog post will be written by Ben Nelson.
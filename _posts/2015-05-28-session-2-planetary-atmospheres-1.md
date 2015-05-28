---
layout: post
title: Planetary Atmospheres 1
description: 
tags: [ERES, Planetary Atmospheres]
image:
  feature: banner.jpg
  credit: ESO, Nathaniel C. Sheetz
  creditlink: 
---

Our first session of planetary atmosphere talks is chaired by PSU graduate student Natasha Batalha (who is also our live-tweeter for the symposium).

---
***Hubble Space Telescope Spectroscopy of WISE Detected Brown Dwarfs* (Adam C. Schneider, University of Toledo)**

The Wide-Field Infrared Survey Explorer (WISE) is an all-sky survey which is maps the sky in four infrared wavelengths, ranging from the near-visible to the mid/far infrared wavelengths. As such, WISE has been very very good at detecting very cool sources that appear bright in the infrared, like brown dwarfs. He's talking today mostly about Y dwarf stars, which are the coolest known brown dwarfs (but still aren't planets). Y dwarfs range from around 400 K to 250 K, which is near the temperature of Earth! Y dwarfs pop out in WISE images as bright green points, and we've found around 20 of them so far.

"Why WISE Ys?" These anchor our low-temperature spectroscopic models, places where "regular" stars don't emit a lot of light. Y dwarfs, because they are near the temperatures of planet can help us understand exoplanets, too. They are the "missing link" or the "crossover" objects. They are so faint that we can't really detect them using ground based telescopes, so we go to space with the *Hubble Space Telescope (HST)* and WISE.

They use *HST* to take spectra of their Y dwarf spectra in the Y-band (Why the Y-band of Wise Ys?) because as you get to lower and lower temperature, there is a very distinctive absorption feature in the ammonia band that appears in the Y-band in spectral models. Their question is: as you go to lower temperatures, why does that absorption feature appear? Where does that ammonia go? Their answer is vertical mixing: the ammonia that would normally appear in the upper layers of the Y-dwarfs and cause that ammonia line are getting mixed into the lower layers, and so there is less ammonia than is expected. However, simultaneously fitting the near- and mid-infrared images is still an issue, as they want to fit all distinctive features at the same time. That issue is ongoing.


---
***Hot Jupiter Atmospheres Revealed with HST/WFC3* (Laura Kreidberg, University of Chicago)**

Transit modeling code: batman = Bad-A* * Transit Model cAlculatioN, currently in development and online at [github](https://github.com/lkreidberg/batman). If you help with testing and debugging, Laura Kreidberg will buy you a beverage.

They are observing HJs WASP-43b and WASP-12b using an *HST* program called "Follow the Water." As the name suggests, they are looking at water bands of these HJs to get precise water abundance estimates. They find about 0.5-.75 times the solar water abundance in WASP-43b. This is important to know because water is a key molecule in planet formation. WASP-43b also very nicely follows the mass-metalicity relation for planets, that more massive planets have fewer heavy elements than less massive planets.

WASP-12b, also a HJ planet, is the "canonical" carbon rich planet, where the C/O ratio is greater than 1 (recall from the last session, most stars have C/O around 0.5). Previous estimates of the C/O ratio are based on emission spectra, and they are taking a transmission spectra (though the atmosphere), and detected a very strong water feature. This is strange because with a high C/O ratio, most of the oxygen should be bound up in carbon monoxide or carbon dioxide, not water. From their transition spectra they find that an oxygen rich model is more accurate than a carbon-rich model. For this, a C/O < 1 is a million times more likely than C/O > 1 (i.e. an oxygen rich model is much much more likely than a carbon rich model).

In the future, they (and we) need to study the whole planet to characterize the atmosphere (not just the temperature/pressure structure, or the atmosphere) but the whole thing at once. We need to reconcile our results from the emission spectra and the transmission spectra. They want to break the degeneracy between models of temperature/pressure and composition. Hopefully breakthroughs will be forthcoming!


---
***Emission and Phase Curves from 3D Exoplanet Atmospheres* (Y. Katherina Feng, UC Santa Cruz)**


Katherina (a recent PSU graduate) is talking about the emission from the planetary atmospheres using 3D model atmospheres. This will help us figure out what kinds of spectra we will be seeing when the *James Webb Space Telescope* finally launches, and so that we can characterize our future observations. *JWST* will be much more precise and accurate in the infrared than current telescopes, so we need to understand what these planet should look like in *JWST* spectra. Doing 3D models will help us figure out what limits our accuracy in detection and modeling, and what biases are inherent in our 1D models.

They are testing a new 3D radiative transfer code "SPARC" to test the opacity grids against the 1D models, and have found that there are some discrepancies. If they use the same opacity grids as the 1D models do, the 3D code and the 1D codes match more closely. They apply this to WASP-43b and find that the assumed inclination of the planet has little effect on the spectral solution (they then assume an edge-on system).

When they look at the atmospheres in a variety of wavelengths and phases, they see that atmospheres are really complex 3D structures, and a 1D analysis of the atmosphere may not cut it. First, is there a difference between the day and night sides of the planets? the 3D model does show differences between the day and night side profiles. Is the 1D model biased towards the day side? Yes, it is. Our measurements in should essentially be an average of the day and night side, but 1D models are more biased towards day side values. They plan to test the limits of exoplanet spectroscopy using their new 3D models and ferreting out the biases in our 1D retrievals.


---
We're going to be changing gears and talking about how to write a successful fellowship or grant proposal with our Fellowship Panel, made up of four successful fellowship winners.
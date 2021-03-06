---
layout: post
title: Instrumentation
description:
tags: [ERES, Instrumentation]
image:
  feature: banner.jpg
  credit: ESO, Nathaniel C. Sheetz
  creditlink: 
---
Good morning everyone and welcome back to the ERES 2015 blog. Our first session this morning in on instrumentation related to exoplanet observations, and is chaired by Yale graduate student, Joseph Schmitt.

---
***The Habitable-zone Planet Finder Instrument: Pushing the Limits of Exoplanet Detection in the Near-Infrared* (Sam Halverson, PSU)**

The Habitable Zone Planet finder is am infrared doppler spectrograph with a 1 m/s precision to find habitable zone planets around M-dwarfs. The HPF team is a very large team spanning multiple universities, and multiple departments at PSU.

Why do we care about radial velocities in the near-infrared? The majority of nearby stars (from the RECONS) survey are M-dwarf stars, which primarily emit light in the NIR. There is a high frequency of planets around these M-dwarfs, almost half of them have at least one planet, and this is a population that is largely untapped by telescopes like *Kepler.* A habitable zone planet around one of these stars would induce an RV signal on the order of meters/second, so this instrument will be ideally placed to measure these RVs in the NIR.

The HPF will be mounted on the Hobby-Eberly Telescope (HET) at McDonald Observatory, of which PSU is a partner. The HPF borrows some of the success of HARPS in its design. It is a fiber-fed spectrograph, with science fibers and calibration fibers. It uses a HgCdTe absorbing detector, not a CCD. The entire spectrograph is contained within a cryostat chamber, similar to the APOGEE instrument. To achieve 1 m/s precision in the NIR, they plan to utilize a laser-frequency comb, but are also looking into a Fabry-Perot etalon for a frequency calibrator, which may be of use to the wider astronomical community rather than tailor-made for the HPF observations. The HPF is exploring a new area of exoplanet detection, piggybacking on the successes of previous instruments like HARPS and APOGEE in its design, and developing cutting edge solutions to the complex problem of high-precision RVs in the NIR.

---
***Ultra Precise Environmental Control for High Precision Radial Velocity Measurements* (Gudmundur Stefansson, PSU)**

The search for habitable planets is exciting! (author's note: indeed!) Improved radial velocity precision enables us to detect lower mass planets, and HPF will focus on HZ planets around M-dwarfs. M-dwarfs are currently our best bet to look for rocky, low-mass planets in the HZ. NIR detector are better suited than optical detectors to study rocky planets around M-dwarfs. HPF is aiming for the same precision as HARPS, but in the NIR instead of the optical.

HPF will push the boundaries of temperature and pressure stabilities achieved by HARPS. Temperature changes cause the echelle groove density to change, which degrades the precision. This can be on the over of 60 cm/s at a 10 mK change in temperature. Their are aiming for a temperature stability of 1 < mK precision in their cryostat. Environmental control is essential to reach 1 m/s RV precision in the NIR. 

The HPF environmental control system opens the path to their 1 m/s goal precision. The components of the environmental control system are largely constructed and fabricated by PSU graduate students. Their actively controlled heaters keep HPF at 180 K with mK stability. They are currently testing and demonstrating the stabilizing effects of their thermal enclosure by testing things at HET. Right now HPF is in mid-integration phase in New York, and they plan to have the integration phase done in a  month or so, whereupon they will proceed to ship the instrument to PSU for further testing.

<iframe width="560" height="315" src="https://www.youtube.com/embed/TViRYUlwiUo" frameborder="0" allowfullscreen></iframe>

---
***Improve RV Precision through Better Spectral Modeling and Better Reference Spectra* (Sharon Xuesong Wang, PSU)**

Detecting Earth is hard, especially in RV. the RV jitter in Keck's HIRES spectrograph for Kepler 78 is ~2 m/s. Their goal is to accurately model the stellar spectrum, and compare them to empirically derived reference spectrum. They then apply a "best guess" RV, convolve the model stellar spectrum with the instrumental PSF, and iterate until they find the best RV needed to match the reference spectrum. This reveals the radial velocity signal within the stellar spectrum, which allows them to detect planets.

There are a number of things that can confuse this straightforward process. Firstly, barycentric correction terms (see Wright & Eastman 2014 for more details on this). But if you are detecting things from the ground, you may be detecting spectral lines that are not from the star itself, but telluric lines from the Earth's atmosphere instead.  The telluric lines won't show the same radial velocity as the stellar lines, which can mess up an RV signal. You need to add telluric lines into your model, or completely mask out regions of telluric contamination, in order to get rid of this. But, there are also *micro-telluric* all over the visible and IR spectrum which cannot be masked out, so you *need* to accurately model the tellurics in order to improve your precision.

Now, they also test the reference spectra of I2 cells at PSU's Hobby-Eberly Telescope, and found that when they tested the I2 cells recently, the reference spectra were different than what they were 20 years ago. This should not be! So they tested again, and found that the newer Fourier transform spectrum of the I2 cell appears to be more accurate than the older one. In the future, they plan to take the improved telluric calibrations and the improved I2 reference spectra to improve the codes used to calculate RVs. They want a Python/GitHub/Bayesian RV code to be implemented, which will improve the precision and accuracy of ground based. RV measurements all around.

<iframe width="560" height="315" src="https://www.youtube.com/embed/_mUheadg9LM" frameborder="0" allowfullscreen></iframe>

---
***First exoplanet transit observations with SOFIA* (Daniel Angerhausen, NASA Goddard)**

Spectrophotometry in 30 seconds: sometimes we are lucky to observe edge on transits, but usually we are looking at grazing or secondary transits which are more difficult to characterize. Spectrophotometry looks at the transit light curve in many many wavelengths and then compiles that into a spectrum: so **spectro-** because they are creating a spectrum, and **photometry** because they are creating these spectra from photometric measurements of transits rather than a traditional spectrograph. This can tell them about the atmospheric composition, and atmospheric structure of HJs.

SOFIA is a telescope on a plane, a Boeing 747-SP aircraft that flies higher than commercial aircraft. It's a good compromise between a ground-based telescope and a space-based telescope: they remove some of the atmosphere (99%) that plagues ground based observations, but they can't observe as often as the ground because of flight restrictions.
 It operates in the NIR (0.3 micron to 1.6 mm). It has a wide wavelength regime and is mobile, which is good all for transit observations. "SOFIA is a space telescope that comes home every day" which lets them continually update the instrumentation on the telescope, something you can't do with space-based telescopes. This means that SOFIA will always have the cutting-edge detection methods (provided that funding exists).

SOFIA had its first exoplanet observation in October 2013 with FLIPO, planet HD189733b, and achieved "space-based" quality of 185/160 ppm precision. As that was the first observation, they expect that the precision and accuracy of their instruments will only improve as they gain further understanding of them. They are currently working on GJ-1214b transit observations. Even when JWST goes up, people will still need alternatives for transit observations, and SOFIA is the perfect not-quite-space telescope.

<iframe width="560" height="315" src="https://www.youtube.com/embed/uxQPNd9cfMg" frameborder="0" allowfullscreen></iframe>

---
***Suborbital Demonstrations of Starshades* (Anthony Harness, University of Colorado-Boulder)**

"The firefly and the lighthouse": an Earth-like planet is 10^10 times fainter than the host star and only 0.1 arcseconds away. This is comparable to trying to detect the light from a firefly that is flying in front of a lighthouse. A starshade is a way to mask out the light from the star and only detect the light from the planet. The benefit to this is that all of the light-masking is taking place outside of you telescope, so if you want full-light measurements (like from a spectrograph) at the same time you can do both at once.

The community needs to do end-to-end system level tests of starshades so that we can prove that it works and and gain confidence amongst the community that starshades are worth it before we spend a lot of time and money making them. The best way to do this is to do real tests with real data on a smaller ground telescope to make a proof-of-concept.

They wanted to try a zepplin - but alas, no such luck. They next moved to a vertical-takeoff, vertical-landing rocket that can hover and be used as a starshade platform for a ground telescope. They want to ensure that the starshade has cm accuracy and stability - if light keeps leaking around the edges, the measurements are ruined. They plan to use two small telescopes: one for measurements and one as a guiding telescope to make sure that the science telescope is still pointed at the star. Rockets are still a bit far off, however, so their first attempts will be a simple stationary starshade on a tall peak that can be angled to follow the star's path, and make use of a somewhat mobile telescope. They plan to attempt the stationary method this summer (2015), and their ultimate goal is to have the telescope 3km away from the starshade and detect the disk around Fomalhaut. Their initial tests have been able to detect a "planet" at a 10^-8 contrast to its "star".

<iframe width="560" height="315" src="https://www.youtube.com/embed/Ugpyftklllc" frameborder="0" allowfullscreen></iframe>

---
***Multiband nulling coronography* (Brian A. Hicks, NASA Goddard)**

"Nuller" - nulling coronograph. This has similar results to a starshade, in that the starlight is "removed" from the image. Instead of directly blocking the light, a nuller works by using destructive interference of the starlight to detect fainter light that light that is also in the images. In order to detect a Jupiter around the Sun, you need 10^-8 contrast, and for Earth you need 10^-10 contrast.  This is a direct-imaging technique to allow you to get down to these precision levels. HZ exo-Earths require very specific inclinations for transits (they essentially must be within a few degrees of edge-on for us to see them transiting), but direct imaging favors "face-on" planet systems rather than edge-on transit systems, so they can probe an entirely different population of planetary systems and reduce our current detection biases.

Direct imaging, because it favors face-on, means that they could observe a planet throughout its "seasons," look at variations in the planetary albedo (reflectivity) over time, and possibly look at the effects of weather patters on exoplanets. If they broaden the search away from "habitable," they could even talk about the "infestible zone," climates where extremiphiles could live. Spectroscopy of directly imaged planets would require a large telescope, and they want to get the spectrum in a large wavelength-range.

In addition to planets, they want to detect debris disks and protoplanetary disks, and observe the evolution of planetary systems through many stages (protoplanetary, planetary, and debris). They want to design a coronograph that could work with a future space-based telescope like JWST and has capabilities in UV, visible, and IR wavelengths. Exo-C and Exo-S are potential future "Exo-coronograph" and "Exo-starshade" missions, both aimed at direct imaging of planets.


---
Time for coffee! And then on to the panel on alternate career paths, moderated by yours truly.
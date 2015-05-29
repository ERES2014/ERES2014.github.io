---
layout: post
title: Instrumentation
description: a description 
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

---
***Improve RV Precision through Better Spectral Modeling and Better Reference Spectra* (Sharon Xuesong Wang, PSU)**

Detecting Earth is hard, especially in RV. the RV jitter in Keck's HIRES spectrograph for Kepler 78 is ~2 m/s. Their goal is to accurately model the stellar spectrum, and compare them to empirically derived reference spectrum. They then apply a "best guess" RV, convolve the model stellar spectrum with the instrumental PSF, and iterate until they find the best RV needed to match the reference spectrum. This reveals the radial velocity signal within the stellar spectrum, which allows them to detect planets.

There are a number of things that can confuse this straightforward process. Firstly, barycentric correction terms (see Eastman & Wright 2014 for more details on this). But if you are detecting things from the ground, you may be detecting spectral lines that are not from teh star itself, but telluric lines from the Earth's atmosphere instead.  The telluric lines won't show the same radial velocity as the stellar lines, which can mess up an RV signal. You need to add telluric lines into your model, or completely mask out regions of telluric contamination, in order to get rid of this. But, there are also *micro-telluric* all over the visible and IR spectrum which cannot be masked out, so you *need* to accurately model the tellurics in order to improve your precision.


---
***First exoplanet transit observations with SOFIA* (Daniel Angerhausen, NASA Goddard)**

---
***Suborbital Demonstrations of Starshades* (Anthony Harness)**

---
***Multiband nulling coronography* (Brian A. Hicks)**

---
Time for coffee! And then on to the panel on alternate career paths, moderated by yours truly.
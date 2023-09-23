# duotransits

### introduction

This project assessed the feasibility of utilising the Windmill Hill Observatory at the University of Warwick to determine the true orbital period of TESS duotransit candidates. By analysing NASA’s TESS mission data, we identified duotransit exoplanet candidates, and generated a range of possible orbital period aliases. Despite facing technical challenges and weather-related setbacks, the observatory demonstrated the potential for ground-based observations of exoplanet transits. The installation of a new camera promises improved data quality. This research project highlights the importance of identifying duotransits visible from the Northern hemisphere and underscores the observatory’s potential for year-round contributions to exoplanet observations.

### transits

When we observe an exoplanetary system nearly edge-on, the planet periodically passes in front of the star, causing an eclipse known as a transit. During this event, the observed brightness (measured as flux) of the star decreases from its baseline as the planet blocks some of the light. In recent years, searching for these transits has proven to be a productive means of discovering new planets, a method known as the transit method. The transit method involves detecting dips in the visible light of stars and requires that planets pass in front of stars along our line of sight. Transit photometry, which records the flux of an object over a given period, provides a wealth of information about a planet.

<img width="515" alt="Screenshot 2023-09-18 at 17 04 36" src="https://github.com/mohummudh/duotransits/assets/137917845/cd058a88-b43f-47be-a13f-5b8f0051602f">

### duotransits and their aliases

Some stars exhibited “duotransits”, where a star shows one transit in Year 1 and one in Year 3 of the mission in its lightcurve. Duotransits require less intensive observation campaigns. They limit possible orbital periods to a discrete set, each called an “alias”. After obtaining these aliases, it is possible to check specific orbital periods via photometric monitoring of the duotransit candidate at specific times. Determining the orbital period is valuable, as it reduces the number of radial velocity measurements needed to confirm and measure the mass of an exoplanet, helps determine the planet’s distance from its star, and whether the planet may be habitable.

This repository hosts the vetting process, the data reduction and cleaning, and the alias creation process.

## TOIcatalogue
This folder shows the process of reducing the TESS Objects of Interest (TOI) catalogue to get a list of duotransits (targets with two observed transits) observable from the Windmill Hill Observatory at the University of Warwick. Reducing the data from 6739 candidates to only 10 possible targets (Dataset from https://tev.mit.edu/data/collection/193/). 

## example
This folder contains a notebook going through the process for cleaning the lightcurves and obtaining aliases for a TESS object of interest (in this code TIC26547036). 

## solvedTIC276376289 - the solved system
This folder contains a notebook going through the same process, here I have shown the system I solved, finding the orbital period for the target (TIC276376289). We later found that this system had been confirmed as an eclipsing binary system, and thus was retired as an exoplanet candidate - still we were successful in determining an orbital period of 30.1174 days was found; and the same value is given in a recent SPOC DV report.

## on the ground
These aliases them formed the basis for creating an observing strategy and schedule to confirm or exclude these possible orbital periods in a step-wise manner, narrowing down onto the true orbital period of the system - a crucial step in confirming exoplanet candidates.

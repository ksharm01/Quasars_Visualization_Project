# Quasar Data Analysis and Visualization Project

## Overview
This project focuses on the analysis and visualization of astronomical data related to quasars. Quasars are highly energetic and luminous objects found at the centers of galaxies, powered by supermassive black holes. Understanding quasars involves studying their brightness variations, positional data, and statistical properties derived from observational data.

## Objectives
The primary objectives of this project include:

* Data Acquisition and Preparation:
Loading and preprocessing astronomical data from sources like CSV and Excel files containing quasar observations.

* Parametric Estimators Analysis:
Calculation of statistical metrics such as weighted mean, chi-square, standard deviation, median absolute deviation, interquartile range, robust median statistic, normalized excess variance, F variance, amplitude of variance, peak-to-peak variability, and von Neumann ratio. These metrics provide insights into the variability, distribution, and reliability of quasar brightness measurements.

* Visualization:
Generating visual representations of the data using histograms, scatter plots, and possibly 3D plots where applicable. Visualizations aid in interpreting the statistical findings and identifying patterns in quasar behavior.

### QUASARS

Quasars, short for "quasi-stellar radio sources," are extremely luminous and energetic objects found at the centers of some galaxies. They appear star-like ("stellar") in optical telescopes but emit vast amounts of energy across the electromagnetic spectrum, from radio waves to X-rays. Here are some key points about quasars:

* Nature: Quasars are powered by supermassive black holes at the centers of galaxies. As matter falls into these black holes, it heats up and emits enormous amounts of radiation.

* Brightness: Quasars are among the brightest objects in the universe. Some can outshine entire galaxies of billions of stars.

* Redshift: Most quasars are observed at large cosmological distances, which causes their light to be redshifted. This redshift indicates they are moving away from us and the universe is expanding.

### RA and DEC

RA (Right Ascension) and DEC (Declination) are celestial coordinates used to specify the position of astronomical objects on the celestial sphere, akin to longitude and latitude on Earth's surface.

RA is analogous to longitude on Earth, indicating how far east an object is located relative to the prime meridian
DEC is analogous to latitude on Earth, indicating how far north or south an object is located relative to the celestial equator.

Usage:

* Coordinates: Together, RA and DEC provide a unique positional reference for any celestial object, allowing astronomers to precisely locate and study stars, galaxies, quasars, and other celestial bodies.
* Mapping: The celestial sphere is divided into grids based on RA and DEC, facilitating the mapping of the sky and enabling astronomers to identify specific objects and study their positions, movements, and interactions.

Information about the CVS files:

## Data Sources:

datafinal2.xlsx: This file contains detailed data regarding quasars, including their coordinates and other relevant information.

2119-53792-0479_graph.csv: This dataset has been sourced from the CALTECH website, utilizing the Right Ascension (RA) and Declination (DEC) values extracted from datafinal2.xlsx to pinpoint specific quasar observations.

## Undertanding & Visualizing the data
This Python script performs analysis and visualization of astronomical data related to quasars using various plotting techniques. It utilizes data from the file datafinal2.xlsx to generate histograms and scatter plots of Right Ascension (RA), Declination (DEC), and Redshift values.

## Plotting the Parametric estimators values
This Python script analyzes and plots various parametric estimators based on astronomical data from 2119-53792-0479_graph.csv. It calculates and prints several statistical metrics related to the brightness (MAG) and its associated error (MAGERR) for quasars.

Calculates and prints the following statistical metrics:

* Weighted Mean: Average brightness weighted by the inverse square of the measurement errors.
* Chi-Square: Measure of the goodness of fit of the weighted mean to the observed data.
* Standard Deviation (σ_w): Weighted standard deviation of the data.
* Median Absolute Deviation (MAD): Median absolute deviation of the data.
* Interquartile Range (IQR): Range between the first and third quartiles of the data.
* Robust Median Statistic (RoMS): Robust measure of the data's variability using median and measurement errors.
* Normalized Excess Variance (σ^2_nxs): Measure of variability relative to the weighted mean.
* F Variance: Square root of the normalized excess variance.
* Amplitude of Variance (σ_m): Amplitude of variability considering measurement errors.
* Peak-to-Peak Variability (v): Ratio of peak-to-peak variation in brightness.
* von Neumann Ratio (η): Ratio of the von Neumann statistic to the weighted standard deviation.

Interpreting Results:
Each metric provides insights into the variability, distribution, and reliability of the quasar brightness measurements.

## Light Curve Program 
Light curves are plots that show how the brightness (magnitude) of an astronomical object changes over time. In this case, we are visualizing data from a CSV file containing measurements of quasars. The script will produce a plot displaying the light curves of the quasars with error bars indicating measurement uncertainties.

#### Dependencies
- pandas
- numpy
- matplotlib
- seaborn
- scipy
- mpl_toolkits.mplot3d

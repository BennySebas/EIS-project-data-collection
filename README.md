# Battery EIS Experimental Data Repository

This repository stores the experimental data generated during the development and validation of the battery analysis system. The data are organized into four main folders, according to their role in the measurement and post-processing workflow.

## Repository Structure


This folder contains the raw and processed data obtained from Electrochemical Impedance Spectroscopy (EIS) measurements.

Typical contents of this folder include:

Frequency points used during the measurement
Impedance magnitude values
Impedance phase values
Real and imaginary impedance components
Averaged results over multiple acquisitions
Measurement metadata, such as date, battery identifier, state of charge, state of health, and test conditions

The files in this folder should allow the reconstruction of Nyquist plots, Bode plots, and any other impedance-based analysis performed in the thesis.

ECM params/

This folder contains the results obtained from Equivalent Circuit Model (ECM) fitting.

Typical contents of this folder include:

Extracted ECM parameter values for each measurement
parameters depending on the adopted model
Fitting cost or fitting error metrics
Information about the fitting conditions, such as the battery state, cycle number, or dataset identifier
Optional comparison between measured and fitted impedance data

The files in this folder should support the analysis of how ECM parameters evolve with battery aging and operating condition.

Calibration data/

This folder contains all data related to the calibration of the EIS measurement system.

Typical contents of this folder include:

Short-circuit calibration measurements
Reference resistor calibration measurements
Transfer functions used for calibration
Measured and expected values for calibration standards
Calibration coefficients applied during post-processing
Metadata describing the calibration setup, date, and reference components used

The files in this folder should allow verification of the calibration procedure and reproducibility of the correction applied to the raw EIS measurements.

Charge Discharge data/

This folder contains the data acquired during controlled battery charging, discharging, and rest periods.

Typical contents of this folder include:

Timestamped voltage measurements
Timestamped current measurements
Coulomb counting data
Temperature measurements, when available
Charge, discharge, and rest state labels
Test configuration parameters, such as charge current, discharge current, voltage thresholds, derivative thresholds, and cycle count

The files in this folder should document the battery cycling procedure and support the analysis of battery aging, capacity evolution, and steady-state detection.

Recommended File Contents

Each dataset file should, whenever possible, include:

Battery identifier
Date and time of acquisition
Test configuration parameters
Measurement units
Clear column headers
Information about the acquisition conditions, such as SoC, cycle number, or temperature
Purpose

The purpose of this repository is to ensure that all experimental data used in the thesis are stored in a structured and reproducible manner, facilitating:

Post-processing
ECM fitting
Calibration verification
Aging analysis
Future reuse of the datasets
Notes
File names should be descriptive and consistent across all folders.
Units should always be explicitly stated.
If both raw and processed versions of the same dataset are stored, this should be clearly indicated in the file name.

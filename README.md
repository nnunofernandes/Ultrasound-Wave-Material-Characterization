# MATLAB Post-Processing Tool for Ultrasound Transmission Measurements in Soft Tissue and Tissue-Mimicking Samples

[![DOI](https://zenodo.org/badge/1246053081.svg)](https://doi.org/10.5281/zenodo.20334339)

## Overview

This repository contains MATLAB post-processing toolbox and code developed for the analysis of ultrasound transmission measurements in soft biological tissues, tissue-mimicking materials, and related acoustic characterization samples.

The software was designed to process experimentally acquired ultrasound signals and extract relevant acoustic parameters from through-transmission measurements. The workflow is particularly suited for experimental setups where a sample is placed between two ultrasound transducers and the transmitted signal is acquired using an oscilloscope.

The code was originally developed to support the acoustic characterization of soft tissue-mimicking materials and anatomical phantom components for ultrasound-based biomedical applications.

## Experimental Setup

The experimental setup was modified based on the principle of an impedance tube, also known as a Kundt’s tube. In this configuration, tissue samples or tissue-mimicking materials are placed between two ultrasound transducers.

The samples are separated by spacer rings with a fixed thickness of 1 mm. This ensures that the sample height remains constant and equivalent to the combined height of the spacers. This configuration allows consistent and non-compressive measurement of acoustic wave propagation through soft samples, reducing variability caused by uncontrolled compression.

<p align="center">
  <img width="3215" height="1568" alt="Experimental setup" src="https://github.com/user-attachments/assets/87124e2d-22d2-41f6-8cf6-b7643513fcf9" />
</p>

## Data Acquisition Assumptions

This software was developed assuming that the desired transmitted ultrasound signal is acquired in the second channel of a Rigol DS1054Z 4-channel oscilloscope.

The original acquisition configuration assumes:

- Oscilloscope: Rigol DS1054Z
- Number of channels: 4
- Signal channel used for post-processing: Channel 2
- Application: through-transmission ultrasound signal analysis
- Measurement condition: fixed sample thickness using non-compressive spacer rings

If needed, the application can be modified to allow generalized signal input from other oscilloscope channels or acquisition systems.

## Main Features

The MATLAB post-processing workflow can be used to support the analysis of ultrasound signals acquired from soft tissue or tissue-mimicking samples. Depending on the available data and user-defined inputs, the code may be used for:

- Importing and processing oscilloscope-acquired ultrasound signals;
- Visualizing time-domain signals;
- Comparing reference and sample-transmitted signals;
- Estimating time-of-flight differences;
- Supporting the calculation of ultrasound propagation parameters;
- Assisting in the characterization of tissue-mimicking materials and biomedical phantoms.

## Intended Applications

This software is intended for researchers working on:

- Ultrasound characterization of materials;
- Development of tissue-mimicking materials;
- Medical phantom fabrication;
- Acoustic property estimation;
- Through-transmission ultrasound testing;
- Biomedical ultrasound device development;
- Experimental validation of numerical acoustic models.

## Example Applications and Related Publications

For examples of sample sizes, experimental procedures, and applications related to this type of acoustic characterization methodology, please consult the following articles:

- https://doi.org/10.3390/jcs9070370
- https://doi.org/10.3390/bioengineering12090946

## Citation

If you use this software in your research, please cite the associated Zenodo archive:

```bibtex
@software{fernandes_matlab_ultrasound_postprocessing,
  author       = {Fernandes, Nuno A. T. C.},
  title        = {MATLAB Post-Processing Code for Ultrasound Transmission Measurements},
  year         = {2026},
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.20334339},
  url          = {https://doi.org/10.5281/zenodo.20334339}
}

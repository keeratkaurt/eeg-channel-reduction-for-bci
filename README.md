# EEG Channel Reduction for Motor Imagery Classification

## Overview
Brain–computer interfaces (BCIs) often rely on large numbers of EEG electrodes to decode neural activity. However, wearable and consumer BCI systems require fewer electrodes to improve usability, comfort, and setup time.

This project investigates how reducing the number of EEG channels affects motor imagery classification performance using public BCI datasets. By training classifiers on the full electrode set and progressively removing channels, we evaluate which electrodes contribute most to decoding motor imagery signals.

The goal is to determine whether accurate motor imagery classification can be achieved with a minimal electrode configuration.

## Research Questions
- How does classification accuracy change as the number of EEG electrodes decreases?
- Which EEG channels contribute most to motor imagery decoding?
- Can motor imagery classification remain accurate with a reduced electrode set?
- What electrode configurations may be optimal for practical wearable BCI systems?

## Dataset
This project uses publicly available motor imagery EEG datasets commonly used in BCI research.

Examples include:
- BCI Competition datasets
- Motor imagery EEG datasets containing left vs. right hand imagery trials

Each dataset contains multi-channel EEG recordings collected while participants perform motor imagery tasks.

## Methods

### Preprocessing
Typical EEG preprocessing steps include:
- Bandpass filtering
- Artifact removal
- Epoch extraction around motor imagery trials
- Normalization or baseline correction

### Feature Extraction
Features may include:
- Power spectral density
- Mu rhythm (8–12 Hz)
- Beta band (13–30 Hz)
- Time-domain EEG features

### Classification
Machine learning models used for classification may include:

- Logistic Regression
- Support Vector Machines (SVM)
- Random Forest
- Neural network models (optional)

### Channel Reduction Analysis
To evaluate electrode importance:

1. Train a classifier using **all EEG channels**
2. Iteratively reduce the electrode set
3. Compare classification performance across different channel configurations
4. Identify channels with the greatest impact on decoding accuracy

This approach helps determine whether accurate classification can be achieved with fewer electrodes.

## Expected Outcomes
- Identification of the most informative EEG channels for motor imagery tasks
- Analysis of performance trade-offs when reducing electrode count
- Insights into electrode configurations for practical wearable BCI systems

## Project Structure

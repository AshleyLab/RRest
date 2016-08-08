The _RRest_ Synthetic Dataset
=============================

### Overview

The _RRest_ Synthetic Dataset consists of simulated ECG and PPG signals which have been modulated by one of the three respiratory modulations:

* Baseline Wander (BW),
* Amplitude Modulation (AM), or
* Frequency Modulation (FM)

It is designed for assessment of respiratory rate (RR) algorithms under ideal conditions, as first described in the article cited below.

### Example

![Exemplary](http://haemod.uk/images/research/pete/resp_mods.png)

### Methods

The dataset was generated using the Matlab &reg; script called _RRest-syn_generator_. Exemplary ECG and PPG beats lasting one second were repeated 210 times, giving a simulated signal lasting 210 s. This signal was then modulated by each of the three respiratory modulations in turn (BW, AM and FM), producing three separate signals. This process was repeated for a range of heart rates (HRs, 30 - 200 beats per minute) and respiratory rates (RRs, 4 - 60 breaths per minute). When the HR was varied, the RR was fixed at 20 bpm. When the RR was varied, the HR was fixed at 80 bpm.

For further details of the methodology please see the article cited below.

### Format

The dataset is provided in three formats:

* Comma-separated value format,
* Matlab &reg; data format, and
* WaveForm DataBase (WFDB) format.

In addition, the script used to generate the data, _RRest-syn_generator_, is provided in Matlab &reg; format (although this can be read as a text file).

### Files

The files are separated into three directories. The data is provided in three directories, one for each format. Within each directory are the files corresponding to each of the 192 generated signals (consisting of 35 signals with the RR fixed at 20 bpm, and 29 signals with the HR fixed at 80 bpm, each repeated three times - once for each respiratory modulation). These files are named as _RRest-syn###_, where ### varies from 1-192.

### Citation

Please cite the following article when using the dataset:

Charlton, P. H., Bonnici, T., Tarassenko, L., Clifton, D. A., Beale, R., & Watkinson, P. J. (2016). An assessment of algorithms to estimate respiratory rate from the electrocardiogram and photoplethysmogram. Physiological Measurement, 37(4), 610–626. [DOI: 10.1088/0967-3334/37/4/610](http://doi.org/10.1088/0967-3334/37/4/610)

### Licence

This dataset is distributed under the CC BY Licence (CC BY 3.0), which is available [here](https://creativecommons.org/licenses/by/3.0/).

### Additional References

The figure shown in this file is adapted from:

1. Addison, P.S. et al.: Developing an algorithm for pulse oximetry derived respiratory rate (RR(oxi)): a healthy volunteer study. Journal of Clinical Monitoring and Computing, 26(1), 45-51 (2012), DOI: 10.1007/s10877-011-9332-y

2. Pimentel, M.A. et al.: Probabilistic estimation of respiratory rate from wearable sensors. in Wearable Electronics Sensors, Springer International Publishing, 15, 241-262 (2015), DOI: 10.1007/978-3-319-18191-2_10

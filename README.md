# 2018 M87 EHT Results: Calibrated Data

**Authors:** The Event Horizon Telescope Collaboration et al.

**Date:** March, 2024

**Primary Reference:** [The Event Horizon Telescope Collaboration, et al. 2024, A&A, 681, A79](https://doi.org/10.1051/0004-6361/202347932)

**Data Product Code:** [2024-D01-01](https://eventhorizontelescope.org/for-astronomers/data)

**Brief Description:**

We release a data set to accompany the M87 Event Horizon Telescope (EHT) Results from the April 2018 observing campaign (EHT Collaboration et al. 2024). The data set is derived from the Level 2 Version 1 (L2V1) of the calibrated data released internally within the collaboration. It is now made public simultaneously with four imaging pipelines used to produce the images in the paper, and one direct modeling pipeline.

This data set contains M87 data for all four bands (b1, b2, b3, and b4) for three of the observed days (April 21st, 22nd, 27th, 2018). Data from the 2018 observations were processed through two independent reduction pipelines (Blackburn et al. 2019, Janssen et al. 2019, Paper III). This release includes the fringe fitted, a-priori calibrated, and network calibrated data from both the EHT-HOPS and CASA rPICARD pipelines. Independent flux calibration is performed based on estimated station sensitivities during the campaign (Koay et al. 2023). A description of the data properties, their validation, and estimated systematic errors is given in Section 3 of the 2018 M87 paper (EHT Collaboration et al. 2024).

The data are time averaged to 10 seconds and frequency averaged over all 32 intermediate frequencies (IFs). All polarization information is explicitly removed. To make the resulting `uvfits` files compatible with popular very-long-baseline interferometry (VLBI) software packages, the circularly polarized cross-hand visibilities `RL` and `LR` are set to zero along with their errors, while parallel-hands `RR` and `LL` are both set to an estimated Stokes *I* value. Measurement errors for `RR` and `LL` are each set to sqrt(2) times the statistical errors for Stokes *I*.

All `uvfits` files are located in the "`uvfits/`" subdirectory. Easy-to-read `csv` and `txt` files are derived from the `uvfits` files and provided in "`csv/`" and "`txt/`", respectively. Finally, the `run.sh` script in the top directory will convert `uvfits` files into `csv` and `txt` files.

The three `tgz` files are gzipped tarballs that contains `uvfits`, `txt`, and `csv` files, respectively. They are included in this repository for convenience.

**File Name Convention:**

The data files are named in the following convention:

    [Data-Release-Tag]_[Source]_[year]_[day-of-year]_[band]_[pipeline]_[stage]_StokesI.[format]

**Station Code Table:**

| UVFITS Code | Station Name                  | Location  |
| ----------- | ----------------------------- | --------  |
| AA          | ALMA                          | Chile     |
| AX          | APEX                          | Chile     |
| GL          | Greenland Telescope           | Greenland |
| LM          | Large Millimeter Telescope    | Mexico    |
| MG          | Submillimeter Telescope       | Arizona   |
| MM          | James Clerk Maxwell Telescope | Hawai'i   |
| PV          | IRAM                          | Spain     |
| SW          | Submillimeter Array           | Hawai'i   |

**References:**

- [EHT Collaboration Data Portal Website](https://eventhorizontelescope.org/for-astronomers/data)
- [The Event Horizon Telescope Collaboration, et al. 2024, A&A, 681, A79](https://doi.org/10.1051/0004-6361/202347932)
- [Blackburn, L., Chan, C.-k., Crew, G., et al. 2019, ApJ, 822, 23](https://doi.org/10.3847/1538-4357/ab328d)
- [Janssen, M., Goddi, C., van Bemmel, I., et al. 2019, A&A, 626, A75](https://doi.org/10.1051/0004-6361/201935181)
- [Koay, J. Y., Romero-Cañizales, C., Matthews, L., et al. 2023, EHT Memo 2023-L1-01](https://eventhorizontelescope.org/for-astronomers/memos)

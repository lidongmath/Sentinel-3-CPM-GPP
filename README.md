# Global Sentinel-3 CPM Gross Primary Production (GPP) Dataset (2016–2024)

This repository provides documentation and data access for the global 8-day **Gross Primary Production (GPP)** dataset generated using the **Chlorophyll-based Canopy Photosynthesis Model (CPM)**. The model uses **Sentinel-3 OLCI-derived canopy chlorophyll content (CCC)** and topographically corrected potential photosynthetically active radiation (`PARpot`). The data are published on Zenodo.

---

## Data access

The complete dataset is available on Zenodo:

- **[Global 8-Day CPM GPP Dataset](https://doi.org/10.5281/zenodo.21530751)**

The annual NetCDF data files are not stored in this GitHub repository.

---

## Data characteristics

- **Variable:** Gross Primary Production (`GPP`)
- **Unit:** gC/m²/day
- **Data type:** `single` (`float32`)
- **Missing value:** `NaN`
- **Spatial resolution:** 0.05°
- **Temporal resolution:** 8-day composite
- **Temporal coverage:** 2016–2024
- **Number of annual files:** 9
- **Time steps per year:** 46
- **Latitude extent:** 90°N to 60°S
- **Longitude extent:** 180°W to 180°E
- **Grid dimensions:** 3000 × 7200
- **File format:** NetCDF

Missing values mainly result from unavailable or invalid Sentinel-3 CCC observations caused by cloud and snow contamination, insufficient valid observations, or retrieval failure. Missing values should not be interpreted as zero GPP.

---

## Retrieval method

The GPP product was generated using the **CCC-based Chlorophyll-based Canopy Photosynthesis Model (CPM)**.

CPM estimates GPP using Sentinel-3 OLCI-derived CCC and topographically corrected potential photosynthetically active radiation (`PARpot`). CCC represents canopy photosynthetic capacity, while `PARpot` represents the potential radiation available for photosynthesis.

---

## File naming

Each annual file follows the naming convention:

`YYYY.nc`

where `YYYY` is the corresponding year, for example:

- `2016.nc`
- `2017.nc`
- ...
- `2024.nc`

Each file contains one `GPP` variable with dimensions of:

`3000 × 7200 × 46`

representing latitude, longitude, and 8-day composite periods, respectively.

---

## Applications

The dataset is suitable for:

- terrestrial vegetation productivity assessment;
- ecosystem carbon-uptake analysis;
- crop, grassland, and forest productivity monitoring;
- seasonal and interannual photosynthesis analysis;
- terrestrial carbon-cycle studies;
- comparison and validation of satellite GPP products.

---

## Citation

Please cite the following publication when using this dataset:

> Li, D., Gitelson, A. A., Schreiner-McGraw, A. P., Desai, A. R., Zhu, Y., Cao, W., & Yu, K. (2026).  
> Chlorophyll-based canopy photosynthesis model: Development and global synergy analysis.  
> *Remote Sensing of Environment, 342*, 115468.  
> https://doi.org/10.1016/j.rse.2026.115468

**Dataset DOI:**  
https://doi.org/10.5281/zenodo.21530751

---

## License

The dataset is distributed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.

---

## Contact

For questions or feedback, please contact:

**Dong Li**  
Technical University of Munich  
Email: dongmath.li@tum.de

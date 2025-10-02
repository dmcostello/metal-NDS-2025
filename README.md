---
editor_options: 
  markdown: 
    wrap: 72
---

# metal-NDS-2025

Provisional data and code release for peer review.

Costello et al. *Anemic streams: Iron and essential trace metals
frequently limit primary producer biomass*.

## List of all files in repository

Raw data files in repository:

`NDSsites.csv`

`chlorophyll.csv`

`benthotorch.csv`

`WQ.csv`

`LULC.csv`

`soilmetalWS.csv`

`A_Fe.tif`

`A_Zn.tif`

Derived data files in repository:

`classify.csv`

Code files in repository:

`figures.Rmd`

`statistics.Rmd`

------------------------------------------------------------------------

## Metadata for files used in `figures.R`

### `NDSsites.csv`

| Parameter    | Definition                          | Units                   |
|------------------|------------------------------------|------------------|
| Stream       | Common name of stream               |                         |
| Region       | Common name for region of study     |                         |
| Year         | Year experiment was completed       |                         |
| Problem      | Descriptor of any problems with NDS |                         |
| Cup_letter   | Unique letter code for stream       |                         |
| Deploy date  | Date of deployment                  | month/day/year          |
| Recover date | Date of recovery                    | month/day/year          |
| Latitude     | Latitude of experiment              | Decimal degree (WGS 84) |
| Longitude    | Longitude of experiment             | Decimal degree (WGS 84) |

### `chlorophyll.csv`

| Parameter | Definition                    | Units    |
|-----------|-------------------------------|----------|
| Site      | Common name of stream         |          |
| Year      | Year experiment was completed |          |
| Sample_ID | Unique sample ID              |          |
| Treatment | NDS nutrient treatment        |          |
| CHLA      | Chlorophyll a biomass         | µg/cm^2^ |

### `benthotorch.csv`

| Parameter | Definition                      | Units    |
|-----------|---------------------------------|----------|
| Site      | Common name of stream           |          |
| Year      | Year experiment was completed   |          |
| Sample_ID | Unique sample ID                |          |
| Diatoms   | Diatom biomass                  | µg/cm^2^ |
| Greens    | Chlorophyte biomass             | µg/cm^2^ |
| Cyanos    | Cyanobacteria biomass           | µg/cm^2^ |
| Treatment | NDS nutrient treatment          |          |
| Total     | Total biomass from all pigments | µg/cm^2^ |

### `WQ.csv`

All values are means of 2-4 grab samples collected during the
experimental period.

| Parameter | Definition                                               | Units |
|----------------|----------------------------------------|----------------|
| Site      | Common name of stream                                    |       |
| Mg_ugL    | Streamwater magnesium (unfiltered)                  | µg/L  |
| Ca_ugL    | Streamwater calcium (unfiltered)                    | µg/L  |
| Fe_ugL    | Streamwater iron (unfiltered)                       | µg/L  |
| V_ugL     | Streamwater vanadium (unfiltered)                   | µg/L  |
| Mn_ugL    | Streamwater manganese (unfiltered)                  | µg/L  |
| Co_ugL    | Streamwater cobalt (unfiltered)                     | µg/L  |
| Ni_ugL    | Streamwater nickel (unfiltered)                     | µg/L  |
| Cu_ugL    | Streamwater copper (unfiltered)                     | µg/L  |
| Zn_ugL    | Streamwater zinc (unfiltered)                       | µg/L  |
| Mo_ugL    | Streamwater molybdenum (unfiltered)                 | µg/L  |
| Cd_ugL    | Streamwater cadmium (unfiltered)                    | µg/L  |
| Se_ugL    | Streamwater selenium (unfiltered)                   | µg/L  |
| NO3_ugL   | Streamwater nitrate (filtered)                      | µg/L  |
| SRP_ugL   | Streamwater dissolved reactive phosphate (filtered) | µg/L  |
| NH4_ugL   | Streamwater ammonium (filtered)                     | µg/L  |
| TDN_ugL   | Streamwater total dissolved nitrogen (filtered)     | µg/L  |
| TDP_ugL   | Streamwater total dissolved phosphorus (filtered)   | µg/L  |
| TN_ugL    | Streamwater total nitrogen (unfiltered)             | µg/L  |
| TP_ugL    | Streamwater total phosphorus (unfiltered)           | µg/L  |
| Alk_mgL   | Streamwater alkalinity (unfiltered)                 | mg/L  |

### `classify.csv`

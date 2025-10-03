# metal-NDS-2025

Provisional data and code release for peer review.

Costello et al. *Anemic streams: Iron and essential trace metals frequently limit primary producer biomass*.

## List of all files in repository

**Code files in repository**

`figures.Rmd`

`statistics.Rmd`

**Raw data files**

[`NDSsites.csv`](https://github.com/dmcostello/metal-NDS-2025?tab=readme-ov-file#ndssitescsv)

[`chlorophyll.csv`](https://github.com/dmcostello/metal-NDS-2025?tab=readme-ov-file#chlorophyllcsv)

[`benthotorch.csv`](https://github.com/dmcostello/metal-NDS-2025?tab=readme-ov-file#benthotorchcsv)

[`WQ.csv`](https://github.com/dmcostello/metal-NDS-2025?tab=readme-ov-file#wqcsv)

[`LULC.csv`](https://github.com/dmcostello/metal-NDS-2025?tab=readme-ov-file#lulccsv)

[`soilmetalWS.csv`](https://github.com/dmcostello/metal-NDS-2025?tab=readme-ov-file#soilmetalwscsv)

[`A_Fe.tif`](https://github.com/dmcostello/metal-NDS-2025?tab=readme-ov-file#a_fetif-and-a_zntif)

[`A_Zn.tif`](https://github.com/dmcostello/metal-NDS-2025?tab=readme-ov-file#a_fetif-and-a_zntif)

**Derived data files**\
See `statistics.Rmd` for information about derivation of these data.

`RR_chl.csv`

`RR_BT.csv`

`RR_diatom.csv`

`RR_chlorophyte.csv`

`RR_cyano.csv`

`classify.csv`

**Model files**\
Outputs of random forest models. See `statistics.Rmd` for information about models.

`rfFe.Rdata`

`rfN.Rdata`

`rfP.Rdata`

`rfZn.Rdata`

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

All values are means of 2-4 grab samples collected during the experimental period.

| Parameter | Definition                                          | Units |
|-----------|-----------------------------------------------------|-------|
| Site      | Common name of stream                               |       |
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

### `LULC.csv`

| Parameter | Definition | Units |
|------------------------|------------------------|------------------------|
| WSAREASQKM | Watershed area | km^2^ |
| SANDWS | Soil sand content | \% |
| CLAYWS | Soil clay content | \% |
| MANUREWS | Mean manure application rate | kg/ha/yr |
| FERTWS | Synthetic nitrogen fertilizer application mean rate | kg/ha/yr |
| CBNFWS | Cultivated biological nitrogen fixation mean rate | kg/ha/yr |
| CHEMWS | Water chemistry index score | Unitless |
| BFIWS | Base flow index | \% |
| NABD_DENSWS | NABD dam density | count/km^2^ |
| RUNOFFWS | Mean runoff | mm |
| NPDESDENSWS | NPDES site density | count/km^2^ |
| SUPERFUNDDENSWS | Superfund site density | count/km^2^ |
| TRIDENSWS | Density of toxic release inventory sites | count/km^2^ |
| PRECIP8110WS | 30-year mean annual precipitation | mm |
| TMEAN8110WS | 30-year mean annual air temperature | °Celsius |
| WWTPALLDENSWS | All wastewater treatment density | count/km^2^ |
| SW_FLUXWS | Surface water nitrogen flux | kg N/km^2^ |
| INORGNWETDEP2008WS | Precipitation-weighted mean annual wet deposition of NH~3~+NO~3~ | kg/ha/yr |
| SN2008WS | Annual mean sulfur and nitrogen wet deposition | kg/ha/yr |
| NWS | Mean lithological nitrogen | \% |
| PCTDECID2019WS | Deciduous forest area | \% |
| PCTCONIF2019WS | Evergreen forest area | \% |
| PCTURBHI2019WS | Developed, high intensity land use area | \% |
| PCTURBMD2019WS | Developed, medium intensity land use area | \% |
| PCTURBLO2019WS | Developed, low intensity land use area | \% |
| PCTURBOP2019WS | Developed, open space land use area | \% |
| PCTCROP2019WS | Row crop area | \% |
| PCTHAY2019WS | Pasture/hay area | \% |
| PCTMXFST2019WS | Mixed deciduous/evergreen forest area | \% |
| MGOWS | Mean lithological magnesium oxide in surface soil | weight % |
| K2OWS | Mean lithological potassium oxide in surface soil | weight % |
| AL2O3WS | Mean lithological aluminum oxide in surface soil | weight % |
| NA2OWS | Mean lithological sodium oxide in surface soil | weight % |
| SIO2WS | Mean lithological silicon dioxide in surface soil | weight % |
| CAOWS | Mean lithological calcium oxide in surface soil | weight % |
| P2O5WS | Mean lithological phosphorous oxide in surface soil | weight % |
| SWS | Mean lithological sulfur in surface soil | weight % |
| FE2O3WS | Mean lithological ferric oxide in surface soil | weight % |
| PERMWS | Mean permeability | \% |
| RCKDEPWS | Mean bedrock depth | cm |
| OMWS | Mean organic matter content in surface soil | \% |
| MINEDENSWS | Mine density | count/km^2^ |
| SEPTICWS | Septic system density | kg/ha/yr |
| NANIWS | Net anthropogenic nitrogen | kg/ha/yr |
| NSURPWS | Nitrogen surplus | \% |
| RDDENSWS | Mean road density | \% |
| COALMINEDENSWS | Coal mine density | count/km^2^ |
| PCTIMP2019WS | Mean imperviousness | \% |
| PTSOURCE | Point source density – Sum of coal mine, mine, waste water treatment plant, NPDES site, superfund site, and toxic release inventory site density | count/km^2^ |
| PCTURB | Sum of high intensity, medium intensity, low intensity, and open space land use | \% |
| PCTFOR | Total forest cover, combining mixed forest cover, evergreen cover, and deciduous cover | \% |
| PCTAG |  | Total agriculture land cover, sum of crop cover and hay/pasture cover |

### `soilmetalWS.csv`

| Parameter | Definition                                | Units    |
|-----------|-------------------------------------------|----------|
| A_Co      | Cobalt concentration in the A horizon     | mg/kg    |
| A_Cu      | Copper concentration in the A horizon     | mg/kg    |
| A_Fe      | Iron concentration in the A horizon       | weight % |
| A_Mo      | Molybdenum concentration in the A horizon | mg/kg    |
| A_Ni      | Nickel concentration in the A horizon     | mg/kg    |
| A_P       | Phosphorus concentration in the A horizon | mg/kg    |
| A_Zn      | Zinc concentration in the A horizon       | mg/kg    |
| C_Co      | Cobalt concentration in the C horizon     | mg/kg    |
| C_Cu      | Copper concentration in the C horizon     | mg/kg    |
| C_Fe      | Iron concentration in the C horizon       | weight % |
| C_Mo      | Molybdenum concentration in the C horizon | mg/kg    |
| C_Ni      | Nickel concentration in the C horizon     | mg/kg    |
| C_P       | Phosphorus concentration in the C horizon | mg/kg    |
| C_Zn      | Zinc concentration in the C horizon       | mg/kg    |
| Top5_Co   | Cobalt concentration in soil top 5 cm     | mg/kg    |
| Top5_Cu   | Copper concentration in soil top 5 cm     | mg/kg    |
| Top5_Fe   | Iron concentration in soil top 5 cm       | weight % |
| Top5_Mo   | Molybdenum concentration in soil top 5 cm | mg/kg    |
| Top5_Ni   | Nickel concentration in soil top 5 cm     | mg/kg    |
| Top5_P    | Phosphorus concentration in soil top 5 cm | mg/kg    |
| Top5_Zn   | Zinc concentration in soil top 5 cm       | mg/kg    |

### `A_Fe.tif` and `A_Zn.tif`

Raster of A horizon soils metals. Provided as 3 bands (RGB). Color represent concentrations in deciles. See Smith et al. 2014 *Geochemical and mineralogical maps for soils of the conterminous United States.* <https://doi.org/10.3133/ofr20141082>

# Compound heatwave drought conditions amplify global fire activity

Code used to generate the figures in:

Kumar, M., Abatzoglou, J. T., Kalashnikov, D. A., Sadegh, M., & Kolden, C. A. *Compound heatwave drought conditions amplify global fire activity.* Submitted to *Geophysical Research Letters*.

## Data

The analysis uses the following datasets, as described in the Methods section of the manuscript:

- MODIS MCD64A1 burned area (Giglio et al., 2018): https://modis-fire.umd.edu/ba.html
- GloCAB cropland burned area (Hall et al., 2024): https://zenodo.org/records/7860452
- ERA5 reanalysis (Hersbach et al., 2020): https://cds.climate.copernicus.eu/
- Terrestrial ecoregions (Olson et al., 2001: https://source.coop/cboettig/ecoregion

## Requirements

Python 3.10 or newer, with numpy, pandas, xarray, netCDF4, scipy, matplotlib, geopandas and cartopy.

## Figures

| Figure | Description |
|---|---|
| [Fig1](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/Fig1) | Map of relative daily burned area (%BA Day⁻¹) for CHD, heatwave-only, drought-only and non-extreme days |
| [Fig2](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/Fig2) | %BA Day⁻¹ for forest vs. non-forest ecoregions (a) and by biome (b) |
| [Fig3](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/Fig3) | Ratio of burned area, 2013–2024 to 2001–2012, for forest vs. non-forest ecoregions (a) and by biome (b) |
| [FigS1](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/FigS1) | Map of the start month of each ecoregion's four-month fire season |
| [FigS2](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/FigS2) | Number of ecoregions by fire-season start month |
| [FigS3](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/FigS3) | Map of forest and non-forest ecoregions |
| [FigS4](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/FigS4) | Difference in %BA Day⁻¹ between CHD and each of the other conditions |
| [FigS5](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/FigS5) | Same as Fig. 1, with drought defined by SPEI-12 |
| [FigS6](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/FigS6) | Same as Fig. 1, with heatwaves defined by the 95th percentile of Tmax |
| [FigS7](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/FigS7) | Share of fire-season burned area (%BA) by condition, forest vs. non-forest ecoregions |
| [FigS8](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/FigS8) | Change in CHD days and in burned area per CHD day, 2013–2024 vs. 2001–2012 |
| [FigS9](https://github.com/mkumar-uci/compound-heatwave-drought-fire/blob/main/FigS9) | Annual burned area and its 5-year moving average by condition, forest vs. non-forest ecoregions |

## Notes

- %BA Day⁻¹ follows Eq. (1) in the manuscript: 100 × (mean annual burned area under a condition) / (mean annual fire-season burned area) / (mean annual number of days in that condition), with means taken over 2001–2024.
- Unburnable and cropland-dominated ecoregions are excluded from the burned-area analyses, as described in the Methods.

## Contact

Mukesh Kumar, University of California, Merced (mukeshkumar@ucmerced.edu)

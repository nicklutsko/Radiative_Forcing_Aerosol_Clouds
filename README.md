This document describes data files containing variables that are calculated in the
analysis presented in “Assessing Effective Radiative Forcing from Aerosol-Cloud
Interactions over the Global Ocean” by Wall et al. (2022). Files ending in
“_monthly_anomalies.nc” are monthly gridded anomalies of cloud, aerosol, and
meteorological fields, and files ending in “_regression_coeffs.nc” are regression
coefficients. The individual files are described below. Variables are described in the
attributes of the data files.

•CERES_monthly_anomalies.nc – Monthly gridded anomalies of cloud
properties and radiative fluxes from CERES FluxByCldType Ed. 4.1. Ocean-
covered grid boxes from the native 1° × 1° grid of the satellite data are selected,
the climatological seasonal cycle and long-term linear trend are removed, and
the anomalies are averaged over a 5° × 5° grid.

•MODIS_monthly_anomalies.nc – Monthly gridded anomalies of cloud
properties and radiative fluxes from MODIS Collection 6 version MYD08_M3
(from the Aqua satellite). Anomalies are computed similarly to the CERES data.
Cloud radiative effects are computed using radiative kernels calculated from the
Rapid Radiative Transfer Model for GCMs (see methods section of Wall et al.
2022). For these data, some variables are computed using only fully cloudy
pixels, using only partly cloudy pixels, or using both fully and partly cloudy pixels.
These cases are labeled “CLD”, “PCL”, and “CLD_PCL”, respectively.

•MERRA2_monthly_anomalies.nc – Monthly gridded anomalies of
meteorological predictor variables and dry sulfate-aerosol mass concentration at
910 hPa from MERRA2 reanalysis. Anomalies are computed similarly to the
CERES and MODIS data.

•CERES_regression_coeffs.nc – Regression coefficients from cloud-controlling
factor analysis representing the sensitivity of low-cloud properties to a local
change in the base-10 logarithm of sulfate concentration at 910 hPa. Regression
coefficients are computed using data from the files
“CERES_monthly_anomalies.nc” and “MERRA2_monthly_anomalies.nc”.

•MODIS_regression_coeffs.nc – Regression coefficients from cloud-controlling
factor analysis representing the sensitivity of low-cloud properties to a local
change in the base-10 logarithm of sulfate concentration at 910 hPa. Regression
coefficients are computed using data from the files
“MODIS_monthly_anomalies.nc” and “MERRA2_monthly_anomalies.nc”.

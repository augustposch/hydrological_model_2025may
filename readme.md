# Hydrological Model

This code was developed for the DOE SBIR "UVDAT" (Urban Visualization and Data Analysis Toolkit) with Northeastern University as the subcontractor to Kitware, Inc. This code is publicly available under the MIT license. Written by Raviraj Dave and August Posch, Northeastern University, May 2025.

This code uses historical time series of precipitation, potential evapotranspiration (PET), and streamflow/runoff/discharge, to calibrate and validate a model that uses daily precipitation and PET to predict daily discharge. This model sits in the middle of a chain of models, such that an extreme precipitation value from a climate downscaling model serves as input here, and the output discharge obtained here helps with hydrodynamical modeling to produce a flood simulation and ultimately an infrastructure resilience simulation.

The hydrological model is a SIMHYD model. Read more about it here: -
-https://ewater.atlassian.net/wiki/spaces/SD50/pages/50135548/SIMHYD+-+SRG

-Bhasme, P., & Bhatia, U. (2024). Improving the interpretability and predictive power of hydrological models: Applications for daily streamflow in managed and unmanaged catchments. Journal of Hydrology, 628, 130421.

Current version is for the Charles River catchment.

To do:
- streamline calibration/validation notebook so all paths are found at the top
- add new notebook to easily run the model and obtain discharge for a new day

# census_privacy
Code, data, and synthetic output for "Bias Effects of Differential Privacy in the Census: Simulation and Analysis


In the `raw_data` folder is a geodataframe of Cook County block groups which can be read in directly. The first several cells of the Jupyter notebook demonstrate the process of turning a census block dataframe into that object.  We do not provide this block-level dataframe.

The `synthetic_data` folder contains 18 pickle files.  Each of these contains the ten synthetic dataframes for a particular choice of parameters.  The naming scheme is `dp_{ε}_{geography}.p` where `ε` is the overall privacy loss budget and `{geography}` is the level which received a low allocation of the budget: `bg` for block group, `tt` for tract, `tg` for tract group, `sc` for subcounty, `cy` for county, and `eq` for an equal distribution.

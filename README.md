# WayDown: **R-package for temporal disaggregation of daily precipitation to sub-huurly scale with stochastic copula - markov chain model** 

**Licence** Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)

**Main reference** - XXX

**Stable version with examples** - https://github.com/hydrovorobey/WayDown/releases/tag/v1.0


**Principal scheme of the framework**
![image](https://user-images.githubusercontent.com/25793656/216564384-7d884138-27ca-4f9c-8606-abb7e67c0706.png)


*The package incorporates:*
- BROOK90 physical lumped hydrological model with a special focus on a detailed representation of vertical water fluxes within the soil-water-plant system at a single site
- used global datasets: land cover (Land Cover 100 m), soil characteristics (SoilGrids250), elevation data (Amazon Web Service Terrain Tiles), meteorological forcing (ERA5, MERRA-2, ECMWF seasonal forecast), vegetation characteristics (MODIS LAI, Global Forest Canopy Height)
- modelling framework for auto download and process initial data, parameterize and run the model, process and save output results

*Technical remarks*:
- installation from GitHub is required
- was tested under R (versions 3.6.0 and 4.2.2)
- following libs are required: copula (>= 1.0-1), markovchain (>= 0.8.5-4), lubridate (>= 1.7.10)
- input precipitation data must be provided in the required format


*Publications*:
- xxx


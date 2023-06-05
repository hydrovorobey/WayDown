# WayDown: **R-package for temporal disaggregation of daily precipitation to sub-hourly scale with stochastic copula - markov chain model** 

[![Github All Releases](https://img.shields.io/github/downloads/hydrovorobey/WayDown/total.svg)]()

**Licence** Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)

**Main reference** - https://hess.copernicus.org/preprints/hess-2023-108/

**Stable version with examples** - https://github.com/hydrovorobey/WayDown/releases/tag/v1.0


**Principal scheme of the framework**
![WayDown_diag](https://user-images.githubusercontent.com/25793656/233024719-b97099b6-79ef-4a93-b42b-9edfc78ad092.png)




*Usage of the package:*
- install the package from GitHub
- install required libs (if necessary)
- load daily (data to disaggregate) and sub-daily (e.g. 1 min, 10 min measured data) precipitation in workspace (data must be provided in specified format, see example)
- select required parameters for convergence and max iteration number
- run the WayDown function - it returns a dataframe with disaggregated time-series

*Technical remarks*:
- package was tested under R (versions 3.6.0 and 4.2.2)
- following libs are required: copula (>= 1.0-1), markovchain (>= 0.8.5-4), lubridate (>= 1.7.10)
- input data requirements: 
    - no missing values are allowed in daily data
    - missing values are allowed in sub-daily data, but the model will freeze/crash if at least few full days with precipitation events (without NAs) will not be found for each month

*Publications*:
- xxx


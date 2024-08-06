# WayDown: **R-package for temporal disaggregation of daily precipitation to sub-hourly scale with stochastic copula - markov chain model** 

[![Github All Releases](https://img.shields.io/github/downloads/hydrovorobey/WayDown/total.svg)]()

**Licence** Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)

**Main reference** - https://doi.org/10.5194/hess-28-391-2024

**Stable version with examples** - https://github.com/hydrovorobey/WayDown/releases/tag/v1.0


**Principal scheme of the framework**
![WayDown_diag](https://github.com/hydrovorobey/WayDown/assets/25793656/5b300688-05c8-432f-8547-153028048a20)





*Usage of the package:*
- download and last release of the package from GitHub
- install package and required libs:
  
   install.packages('copula')
   install.packages('markovchain')
   install.packages("path_to_package/WayDown/", repos=NULL, type="source")

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
- Simulating sub-hourly rainfall data for current and future periods using two statistical disaggregation models – case studies from Germany and South Korea
Ivan Vorobevskii, Jeongha Park, Dongkyun Kim, Klemens Barfus, and Rico Kronenberg, 2024, HESS, https://doi.org/10.5194/hess-2023-108


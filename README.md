# WayDown: **R-package for temporal disaggregation of daily precipitation to sub-hourly scale with stochastic copula - markov chain model** 

**Licence** Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)

**Main reference** - XXX

**Stable version with examples** - https://github.com/hydrovorobey/WayDown/releases/tag/v1.0


**Principal scheme of the framework**
![image](https://user-images.githubusercontent.com/25793656/216564384-7d884138-27ca-4f9c-8606-abb7e67c0706.png)


*Usage of the package:*
- install the package from GitHub
- install required libs (if necessary)
- load daily and sub-daily (e.g. 1 min, 10 min) data of precipitation in workspace (data must be provided in specified format)
- select required parameters for convergence and max iteration number
- run the WayDown function - it returns a dataframe with disaggregated time-series

*Technical remarks*:
- package was tested under R (versions 3.6.0 and 4.2.2)
- following libs are required: copula (>= 1.0-1), markovchain (>= 0.8.5-4), lubridate (>= 1.7.10)

*Publications*:
- xxx


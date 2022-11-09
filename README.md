# West Nile

## Contents

This repository contains data extracted from the [Italian National Institute of Health (ISS)](https://www.epicentro.iss.it/westnile/bollettino) bulletins starting from the summer-autumn season 2012


## Data dictionary

### 

| Column      | Definition | Format     |
| :---        |    :----:   |          ---: |
| Week     |  Week of reporting       | YYYY-WW   |
| Region code| NUTS 3 region code | String |
| Region name | Region of infection name. | String |
| Province code | NUTS 3 province code | String |
| Province name | Province of infection name. | String |
| New human infections | Daily number of new human cases. | Numeric |
| Total number of human infections	 | Cumulative number of human cases.	 | Numeric |
| New human deaths | Daily number of new human deaths. | Numeric |
| Total number of human deaths	 | Cumulative number of human deaths.	 | Numeric |
| New outbreaks in equids | Daily number of equid cases. | Numeric |
| Total number of outbreaks in equids	 | Cumulative number of equid cases.	 | Numeric |
| New deaths in equids | Daily number of equid deaths. | Numeric |
| Total number of deaths in equids	 | Cumulative number of equid deaths.	 | Numeric |
| New outbreaks in birds | Daily number of bird cases. | Numeric |
| Total number of outbreaks in birds	 | Cumulative number of bird cases.	 | Numeric |
| Avg Temp	 | Average temperature a region/province of infection. | Numeric |
| Hum	 | Humidity of a region/province of infection. | Numeric |
| Precip	 | Rainfall intensity of a region/province of infection. | Numeric |


## Getting the data

**Direct download (CSV)**: https://raw.githubusercontent.com/fbranda/west-nile/main/Surveillance_data_West_Nile_virus_infection_regional.csv

**Python** (requires `pandas`):
```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/fbranda/west-nile/main/Surveillance_data_West_Nile_virus_infection_regional.csv")
```

**R** (requires `httr`):
```r
library(httr)
df <- read.csv(text=content(GET("https://raw.githubusercontent.com/fbranda/west-nile/main/Surveillance_data_West_Nile_virus_infection_regional.csv")))
```


## License and attribution

This repository and data exports are published under the CC BY 4.0 license.



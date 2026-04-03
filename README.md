# Hospital Patient Timeline Plot

R script for visualising the spatial and temporal 
relationship of patients during hospital outbreak 
investigation, as described in the publication:

[Akintayo et al. (2024) mSystems](https://journals.asm.org/doi/full/10.1128/msystems.01128-24)


## What it does
- Plots patient ward movements over time
- Colour codes each ward
- Marks date of positive swab for each patient
- Generates publication-ready SVG figures

## Requirements
R packages:
- vistime
- tidyverse
- RColorBrewer
- scales
- cowplot
- pals

Install with:
install.packages(c("vistime", "tidyverse", 
                   "RColorBrewer", "scales", 
                   "cowplot", "pals"))

## Input
Ward movement data with columns:
- Patient
- Ward
- start (date)
- end (date)
- swab_date

## Output
- Timeline plot (SVG)
- Legend plot (SVG)

## Usage
source("Timeline-script-290424.R")

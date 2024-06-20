Original raw data tables:
- Raw folder: lazy_coral_O2_ALL.csv (all O2 measurements)
- Raw folder: lazy_coral_fragment_surface-volume (3D scans data on surface area and volumn of coral fragments)
- Raw folder: dataentry_notes.csv (notes during incubations)
- Titrationen folder: Alkalinity_Day... (all raw outputs of the titrator for alkalinity calculations)
- Titrationen folder: Titration_summaries (files to match titration output with incubations)


R version 4.3.1 (2023-06-16 ucrt)
Order Scripts:
(- Install Packages) # only for the first time
- Preparation Oxygen Measurements (Outlier detection, calculation of photosynthesis and respiration)	-> new data table 'O2_comp.csv'
- Preparation Total Alkalinity (Calculate TA from Titrator output)					-> new data table 'TA_Results_AllDays.csv'
- Preparation Calcification Rate (Calculate calcification rate, Outlier detection)			-> new data table 'O2_and_Calc_comp.csv'
- Preparation Expected Value (calculation of expected value)						-> new data table 'All_expectedvalues.csv' (used in all the analysis scripts)
- Monoculture analysis (All analysis based on the monoculture incubations)					
- Measured vs Expected (All analysis of conspecific, family, diversity and biomass incubations between measured and expected values)
- Link Poly_monoculture (Analysis of link between monoculture and diverse heterospecific incubation performance inc. Blomqvist adjustment)
(- Extra_not_in_manuscript (some extra sanity check graphs))


# all used packages
install.packages(c("tidyverse",
                   "lubridate",
                   "ggpubr",
                   "oce",
                   "rstatix",
                   "patchwork",
                   "nlme",
                   "multcomp",
                   "car",
                   "emmeans",
                   "ggtext",
                   "ggrepel",
                   "MuMIn"
))


 




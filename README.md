# Dungeons & Dragons 2024 Spells: An Analysis in R

A data analysis of every spell in the Dungeons & Dragons Free Rules (2024 Edition), looking at how spell lists differ between classes and how casting speed relates to spell range.

## Questions

1. **How do spell rosters differ across the eight casting classes?**
   Compares roster size, cantrip availability, and spell level distribution for the bard, cleric, druid, paladin, ranger, sorcerer, warlock, and wizard.

2. **Are longer-casting spells more likely to have a feet or sight range?**
   Groups spells by casting speed (fast vs. slow) and range type to test a common gameplay intuition: quick spells are for combat, slow spells are for utility.

## Key Findings

- Wizard and sorcerer have the largest spell rosters, while ranger and paladin have the smallest, partly because neither class gets any cantrips.
- Classes with larger rosters have spells spread more widely across levels; smaller rosters are concentrated at lower levels.
- Fast-casting spells are noticeably more likely to have a feet or sight range than slow-casting spells, and this pattern holds across spell levels.


## Data

The dataset comes from the [TidyTuesday project](https://github.com/rfordatascience/tidytuesday) (released 2024-12-17) and was compiled by Jon Harmon ([@jonthegeek](https://github.com/jonthegeek)) from the official D&D Free Rules. It contains **314 spells** and **27 variables**, including school of magic, level, casting mechanics, range, duration, class availability, and descriptions.

The data is loaded directly from the TidyTuesday repository, so no download is needed.

## Tools

- **R** with the tidyverse: `dplyr`, `tidyr`, `stringr`, `forcats`, `readr`
- **ggplot2** for visualization
- **R Markdown** for the report

## How to Reproduce

1. Clone this repository:
   ```bash
   git clone https://github.com/bluelliam/YOUR-REPO-NAME.git
   ```
2. Install the required package in R:
   ```r
   install.packages("tidyverse")
   ```
3. Open `D&D_Data_Analysis.Rmd` in RStudio and click **Knit**, or run:
   ```r
   rmarkdown::render("D&D_Data_Analysis.Rmd")
   ```

# California Bat Diversity: A Citizen Science Analysis
Final Project - EDS 240: Data Visualization

A data-driven infographic exploring bat observations across California using citizen science data from iNaturalist. The central narrative examines who California bats are, when they're most active, and where they're spotted, told through three complementary visualizations assembled in Affinity Designer.

[Read the full blog on my website](https://iidonaji.github.io/posts/2026-03-08-EDS240-blog/)

# Learning Goals

- Identify which types of visualizations are most appropriate for the data used and target audience
- prepare (e.g. clean, explore, wrangle) data so that it’s appropriately formatted for building data visualizations
- build effective, responsible, accessible, and aesthetically-pleasing visualizations using the R programming language, and specifically {ggplot2} + ggplot2 extension packages
- Write code from scratch and read and adapt code written by others
- apply a DEI (Diversity, Equity & Inclusion) lens to the process of designing data visualizations
- assess, critique, and provide constructive feedback on data visualizations

## Data Source

Observation data queried from the [Calbat iNaturalis Project](https://www.inaturalist.org/projects/calbats), spanning 1998-2025.

 > ** Note:** iNaturalist data reflects observer effort- areas with higher human population denisty tend to show more reported sightings, not necessarily higher bat activity. 


## Visualizations

| Plot | Type | Key Finding |
|------|------|-------------|
| Bat sightings across California | Kernel density map + observation points | Sightings cluster along the coast and Bay Area |
| Most documented bat species | Stacked bar chart | Mexican Free-tailed Bat dominates with 251 observations |
| Seasonal observation patterns | Radial/polar chart | April is the peak month for bat sightings |

## Required R Packages

```r
library(tidyverse)
library(sf)
library(tigris)
library(spatstat)
library(stars)
library(ggplot2)
```

## Repository Structure

```
.gitignore
README.html
README.md
drafting-viz.qmd
exploration.qmd
final-draft.qmd
images/CABat.png
images/Seasonalobs.png
images/bat_sightings.pdf
images/bat_sightings.png
images/bat_sightings2.pdf
images/batemojies.png
images/layoutinspo.png
images/seasonobs.pdf
images/sketch.jpg
images/top-species.pdf
images/top_species.pdf
images/top_species.png
index.qmd
medrano-eds240-infographic.Rproj

```

## Design Notes

- Final infographic assembled in **Affinity Designer**
- Typography: **Century Schoolbook** (titles) + **Garamond** (body text)
- Background: dawn gradient transitioning from night sky to warm morning light
- Colorblind-friendly palettes used throughout; alt text written for all visualizations
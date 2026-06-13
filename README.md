# Monroe County Crash Analysis, 2012–2024
[English](README.md) | [简体中文](README_zh-CN.md)

## Overview

This repository contains exploratory, statistical, and geospatial analyses of motor-vehicle crashes in Monroe County, New York, from 2012 through 2024.

The project was completed by **DSCC 383W Group 1 at the University of Rochester** in collaboration with **Reconnect Rochester**. The analysis emphasizes **fatal and serious injuries (FSIs)** and **vulnerable road users**, including pedestrians and bicyclists.

The project examines four main questions:

1. How does time of day relate to crash frequency and crash severity?
2. Do crash outcomes differ across roadway jurisdictions?
3. Which roadway corridors have elevated fatal and serious injury risk?
4. Did selected road-improvement projects produce measurable safety changes?

## Data Files Referenced by the Notebooks

| File                                                       | Purpose                                                |
| ---------------------------------------------------------- | ------------------------------------------------------ |
| `merged.csv`                                               | Legacy merged version used by the exploratory analysis |
| `2012-24_Crash_Events_std_street_names_dataset.csv`        | Main standardized crash dataset                        |
| `2012-24_Crash_Events_standardized_corridored_dataset.csv` | Standardized dataset containing corridor fields        |
| `pedestrian_cyclist_collisions_all.csv`                    | Pedestrian and bicyclist crash subset                  |
| `AllRoads.csv`                                             | Roadway inventory and jurisdiction information         |

## Data Availability

The source and processed datasets referenced above are not included in this GitHub repository because the files are too large to upload directly.

The notebooks retain the original filenames to document the project workflow. To reproduce the analysis, users must obtain the corresponding datasets and update the local file paths when necessary.

The repository primarily contains the analysis notebooks, code, visualizations, and final report.

## My Contribution

**My contributions are represented in the notebooks and analysis files included in this repository.**

The work contributed to the project includes data processing, exploratory data analysis, statistical analysis, visualization, interpretation of results, and preparation of project documentation.

Because this was a collaborative team project, the repository distinguishes individual analytical work from the overall findings produced by the full group.

## Key Findings

* **Crash frequency and crash severity followed different time patterns.** Total crashes peaked around the afternoon commuting period, particularly near 5:00 p.m., with a smaller morning peak around 7:00–8:00 a.m. However, crashes occurring late at night and in the early morning were more likely to result in a fatal or serious injury.

* **Vulnerable road users faced substantially greater injury severity.** The logistic regression analysis found that crashes involving pedestrians or bicyclists had approximately **11.23 times the odds** of resulting in a fatal or serious injury compared with crashes involving non-vulnerable road users, after accounting for roadway jurisdiction.

* **Jurisdiction was statistically associated with crash severity, but the practical effect was generally small.** Differences were observed across City/Village, County, State, Town, Thruway, and State Park roads. However, most differences in fatal and serious injury rates were modest, and some jurisdiction groups contained relatively few observations.

* **High-risk roadway corridors were identified using fatal and serious injuries per kilometer.** The corridor analysis distinguished intersections, near-intersection areas, and non-intersection road segments. Shorter corridors generally had higher median FSI counts, with the relationship between corridor length and severity changing at approximately **0.95 kilometers**.

* **Apparent crash factors differed across road-user groups.** Inattention, Failure to Yield, and Unsafe Speed were among the most common recorded factors. Inattention was more strongly represented in pedestrian crashes, while Failure to Yield was more strongly associated with bicyclist crashes.

* **Most road-improvement projects did not show statistically significant changes in fatal and serious injuries.** The East Avenue road diet was associated with a statistically significant reduction in total crashes, but not in FSI outcomes. The Elmwood Avenue road diet, Lake Avenue resurfacing project, and Dewey–Driving Park intersection realignment did not show statistically significant changes under the simple before-and-after analysis.

* **The findings should be interpreted as preliminary associations rather than causal effects.** The analysis did not include traffic-volume data, and some project comparisons may have been affected by changes in travel behavior during the COVID-19 pandemic.


## Group 1 Memebers

* Fernando Lopez
* Justin Li
* Barry Magenya
* Cloud Xiao
* Songtao Zhang

## Acknowledgements

This project was completed as part of **DSCC 383W at the University of Rochester** in collaboration with **Reconnect Rochester**.

The original crash data was provided for academic analysis and is not owned by the project contributors.

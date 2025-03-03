# Boating Accidents Analysis

## Background
This project analyzes boating accident data over multiple years to identify trends, common causes, and risk factors. The dataset includes information about accident locations, times, causes, injuries, and fatalities.

## Motivation
Understanding boating accidents is crucial for improving safety regulations, guiding policymaking, and raising awareness about common hazards. By identifying patterns in the data, this project aims to support efforts to reduce accidents and improve maritime safety.

## Data Cleaning Steps
- Standardized inconsistent text formatting (e.g., converting all-caps entries to title case)
- Filtered out null or missing values for key columns such as `InjuredGender`
- Recoded categorical variables (e.g., converting `DayNight` from `-1` and `0` to `Day` and `Night`)
- Combined datasets from different years for longitudinal analysis
- Removed duplicate entries and standardized date formats

## Summary of Findings
- The highest number of accidents occurred during **weekends**, particularly **Saturdays and Sundays**.
- The majority of accidents happened during the **daytime**.
- **Collisions with fixed objects** and **falls overboard** were among the most common accident types.
- A significant proportion of fatalities were linked to **alcohol consumption**.
- Safety measures such as wearing life jackets had a strong correlation with survival rates.

## Code
The analysis was conducted using **Malloy**, a powerful query language for structured data analysis. The following Malloy files were used to separate boating accidents by timeframe:
- `boating-accidents-2009-2013.malloynb`
- `boating-accidents-2014-2022.malloynb`
- `boating-accidents-2023.malloynb`
- `boating-accidents.malloy`

These files contain all data transformations, visualizations, and queries used in this project.

## How to Build Upon This Work
- Expand the dataset to include more recent years for trend analysis.
- Incorporate external data sources, such as weather conditions, to analyze their impact on accident rates.
- Apply machine learning techniques to predict accident likelihood based on key risk factors.
- Develop an interactive dashboard to visualize trends dynamically.

## Visualizations
Below are five of the most important visualizations generated during the analysis:

![Visualization 1](png\viz1-winddamage.png)
- This shows how wind did not result in most damage. Surprisingly no wind caused most damage. Probably because more people were out in water during no wind.

![Visualization 2](png\viz2-ageaddmitted.png)
- Younger people were addmitted to hospital more often than older people.

![Visualization 3](png\viz3-numlifejackets.png)
- As bodies on board increase, so do number of life jackets available. This is good!

![Visualization 4](png\viz4-weatherconsult.png)
- Older people tend to consult weather prior to going out. Maybe the younger generation could learn from this.

![Visualization 5](png\viz5-winddamage2023.png)
- Opposite to results in 2009-2013, 2023 shows strong winds caused most damage, with no winds caused least damage.

## Licensing
This project is released under the **MIT License**, allowing others to build upon this work with proper attribution.


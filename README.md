# netflix-content-strategy-update
Updated analysis of Netflix content strategy using title-level data up to 2025.

---

## Introduction
This project analyzes the evolution of Netflix’s content strategy using title-level data
covering movies and TV shows available up to 2025.

Building on an earlier exploratory team project completed in 2022, this updated analysis
adopts a more structured, strategy-oriented perspective. Rather than focusing solely on
descriptive trends, the project examines how Netflix’s content composition, globalization
patterns, and acquisition scale have evolved over time, with an emphasis on strategic
decision-making reflected in the timing and characteristics of content additions.


## Research Questions
This project focuses on the following questions:

1. Has Netflix shifted its content composition from movies toward TV shows over time?
2. Has Netflix’s content portfolio become more global in terms of production countries?
3. How has Netflix’s movie acquisition strategy evolved in terms of budget and revenue scale over time?


---

## Data
This project builds on insights from a team project completed in 2022
for the CDS 301 (Introduction to Data Science) course.
The original repository focused primarily on exploratory visualization
and descriptive interpretation.

The current project revisits the same domain with updated data and a
more explicit analytical framework, emphasizing temporal trends,
comparative composition, and strategic interpretation.


### Background

This project builds on insights from a team project completed in 2022
for the CDS 301 (Introduction to Data Science) course.
The original repository focused on exploratory visualization and interpretation.

- Original team project repository: [Netflix Global Trends (CDS 301)](https://github.com/pcw419/netflix-global-trends)



---

## Methodology
The analysis follows a structured workflow consisting of data cleaning,
exploratory data analysis (EDA), and research question–driven investigation.

- Data cleaning focused on handling missing values and resolving semantic
  differences between movies and TV shows.
- Exploratory analysis was used to examine distributional properties of key
  numerical variables, revealing strong right-skewness and motivating the use
  of median-based statistics and log transformations.
- Time-based aggregation (monthly, yearly, and quarterly) was applied
  selectively depending on the research question, with quarterly analysis
  used to capture strategic inflection points that are obscured at coarser
  temporal resolutions.

All analyses were conducted using Python, with pandas and matplotlib as
the primary analytical tools.


---

## Key Findings

### Q1: Movies vs TV Shows  
- Netflix’s content additions have maintained a relatively balanced composition between movies and TV shows over time.
- On a monthly basis, both categories generally account for approximately 40–60% of total titles added, indicating no strong dominance by either format.
- While short-term fluctuations are visible, these variations appear to be driven by release timing and batch updates rather than a long-term strategic shift.
- Anomalies observed in the most recent periods are likely influenced by incomplete or uneven data coverage, rather than reflecting an actual change in Netflix’s content strategy.

### Q2: Globalization  
- Netflix established a globally diverse production network early in its expansion phase, with content produced across a wide range of countries from the beginning.
- Over time, the number of production countries does not show a consistent upward trend, suggesting a shift from geographic expansion to stabilization and strategic adjustment.
- Movies are produced across a broader set of countries than TV shows, indicating that films are used as a flexible channel for experimenting with new markets and regional content.
- TV shows exhibit a more stable and concentrated production pattern, reflecting higher investment costs and a preference for proven markets.
- Overall, Netflix’s globalization strategy appears to have evolved from rapid expansion toward selective diversification and portfolio optimization rather than continuous geographic growth.

### Q3: Movie Acquisition Scale (Budget and Revenue)
- Netflix’s movie acquisition budgets have increased steadily over time, indicating a clear shift toward higher-budget content.
- While median revenues also rise in the long run, they fluctuate more strongly than budgets, suggesting growing variability in financial outcomes.
- Quarterly analysis reveals strategic inflection points that are obscured in annual aggregates, including periods of accelerated spending and heightened revenue uncertainty.
- Several quarters show rising acquisition budgets without proportional revenue growth, implying a strategic focus on long-term catalog value, franchise potential, and brand positioning rather than immediate returns.
- Overall, Netflix’s acquisition strategy reflects an increasing willingness to absorb short-term revenue volatility in exchange for higher-scale and strategically valuable content.

---

## Limitations  

### Q1
Because this dataset contains a fixed number of movie and TV titles for each release year, it does not allow for meaningful analysis of absolute growth in Netflix’s content volume over time. Instead, this analysis emphasizes changes in relative composition and proportional trends between movies and TV shows.

### Q2
This analysis uses the number of distinct production countries as a proxy for globalization, which captures geographic breadth but not the volume or intensity of production in each country. As a result, all countries are weighted equally regardless of their actual contribution, and co-productions are not fully distinguished. The findings therefore reflect the breadth of Netflix’s global reach rather than the depth of production in specific regions.

### Q3
Budget and revenue data may be incomplete and reflect overall box office performance rather than Netflix-specific returns. Quarterly fluctuations can also be influenced by small sample sizes, so results indicate strategic tendencies rather than exact financial outcomes.

---

## Reproducibility

This project was developed using a Python virtual environment.
A `requirements.txt` file is provided to ensure reproducibility
of the analysis environment.

All data files are accessed using relative paths to maintain
cross-platform compatibility.

---

## References

- OTT, Video Streaming PLarforms - Revenue and Users[from kaggle](https://www.kaggle.com/datasets/azminetoushikwasi/ott-video-streaming-platforms-revenue-and-users?select=LibrarySize.csv)


- Netflix Movies and TV Show till 2025[from Kaggle](https://www.kaggle.com/datasets/bhargavchirumamilla/netflix-movies-and-tv-shows-till-2025?select=netflix_tv_shows_detailed_up_to_2025.csv)

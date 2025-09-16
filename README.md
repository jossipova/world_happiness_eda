# What Makes People Happy?
*An exploratory data analysis* 

## Introduction & Goal

Have you ever wondered what truly makes a country happy?

We'll be exploring the 2018-2019 World Happiness Report to uncover the key drivers of happiness, and to demonstrate that "softer" social factors can be just as, or even more, influential than economic prosperity.

### Research Questions
- Which factors have the strongest link to happiness?
- How do strongest factors contribute to happiness?
- What separates the happiest countries?
- Does corruption undermine happiness?
- Can other factors make up for lower GDP?

## Data

**Data source:** [World Happiness Report (2018-2019)](https://www.worldhappiness.report/)

### Initial cleanup:
- Removed irrelevant index columns ("Unnamed: 0.1" and "Unnamed: 0")
- Renamed columns for clarity and consistency
- Split the dataset into two separate DataFrames for 2018 and 2019

### Handling missing data:
- Dropped "Healthy life expectancy" column since 98% of its data was missing
- Imputed missing "Perceptions of corruption" value for UAE with the score from the following year, assuming a consistent trend

## Global Happiness Map

These maps highlight how happiness is distributed around the globe in 2018 and 2019, showing which regions are home to the happiest (and least happy) countries.

![Global Happiness Maps](images/global_happiness_maps.png)

## Which Factors Have the Strongest Link to Happiness?

These correlation matrices show that **GDP per capita and social support have the strongest link to happiness**.

On the other hand, factors like generosity and perceptions of corruption have a much smaller effect on the overall happiness score.

This tells us that a country's economic strength and how its citizens feel about the support they receive from their government are the biggest drivers of well-being.

![Correlation Matrix](images/correlation_matrix.png)

## How Do Strongest Factors Contribute to Happiness?

Focusing on 2018, these scatterplots provide a closer look at the previous heatmap, with regression lines highlighting the strong positive relationships between GDP, social support, freedom of choice, and happiness.

![Scatterplots](images/scatterplots_strongest_factors.png)

## What Separates the Happiest Countries?

These charts show what sets the happiest countries apart from the least happy.

**The biggest differences lie in GDP per capita and social support.**

This shows that the happiest nations are not just wealthier, but also have stronger systems of government support.

![Happiest vs Least Happy](images/happiest_vs_least_happy.png)

## Does Corruption Undermine Happiness?

Surprisingly, these plots show that **perceptions of corruption are highest among the happiest countries**.

This could mean that:
- Transparency in these countries leads to a greater awareness of corruption, OR
- Strong social and economic factors can build a resilience to it

![Corruption Analysis](images/corruption_analysis.png)

## Can Other Factors Make Up for Lower GDP?

These charts prove that **a high GDP is not the only path to happiness**.

For some countries in 2018, social support helped achieve a high level of well-being, showing that 'softer' factors can compensate for lower economic output.

![GDP Compensation](images/gdp_compensation.png)

## Conclusion

Our analysis of the 2018-2019 World Happiness Report shows that **both economic and social factors shape well-being**.

**Key Findings:**
- GDP, social support, and freedom of choice stand out as the strongest drivers of happiness
- 'Softer' factors can sometimes compensate for lower economic output
- Overall, happiness is shaped by feeling supported, having the freedom to make choices, and living in a society that cares for its citizens

**Well-being is about more than just money.**

## What's Next?

### Future Analysis Opportunities:
- **Regional or cultural comparisons:** Compare happiness drivers across continents or cultural clusters to see how economic and social factors vary around the world
- **Trends over time:** Extend the analysis to more years to observe how the importance of key drivers changes or stays consistent over time
- **Happiness inequality within countries:** Examine variation in happiness scores within countries and explore whether inequality affects overall well-being (if data allows)

---

## Tools & Technologies Used
- Python
- Pandas for data manipulation
- Matplotlib/Seaborn for visualization
- Jupyter Notebooks for analysis

## Files in this Repository
- `world_happiness_analysis.ipynb` - Main analysis notebook
- `data/` - Raw and cleaned datasets
- `images/` - Visualizations and charts
- `README.md` - This file

---

*Thank you for exploring this analysis! Feel free to reach out with any questions or suggestions.*
```

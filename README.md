# Final_Assignment
## Aim of the Analysis
This analysis explores whether NHL players are disproportionately born in the early months of the year, and whether this trend is specific to the NHL or reflects general national birth trends in Canada. The project also compares birth month distributions between Canadian and non-Canadian players and evaluates whether this distribution could relate to age cutoffs in youth sports.

## How to Run the Code
1. Open the notebook: 'Final_Assignment_Appio.ipynb' in Google Colab
2. Make sure the runtime is set to R before running any cells
   - Go to Runtime at the top of the screen (just below the notebook     title) and check if it is set to R
3. Run each code cell top to bottom - code will not work if you do not run it in order

## Dependencies
I used the following packages in R:
1. 'reader'
2. 'dplyr'
3. 'ggplot2'

These packages should be pre-installed in the R-Colab workspace. 

If they are not use:

- install.packages("readr")

- install.packages("dplyr")

- install.packages("ggplot2")

## Summary of Results
With the rich dataset provided by the TidyTuesday repository, I created several data visualizations to explore birth month trends among NHL players.

The initial visualization revealed a clear trend: a disproportionate number of NHL players are born early in the year, particularly in the first quarter (January–March). As the year progresses, the number of NHL player births noticeably declines, suggesting a possible relative age effect — where older children in youth leagues (due to earlier birth months) may have developmental advantages.

To further explore this, I examined team-level trends by focusing on the 2022–2023 season. I identified which NHL teams had the most Q1-born players, raising the question of whether such teams might perform better — an idea that could be investigated by comparing team performance and birth month distribution.

Next, I compared this NHL trend to Canadian national birth records from 1991–2022. While there is some seasonality in national births, NHL players are far more likely to be born in early months than the general Canadian population. A Chi-Square Goodness of Fit test confirmed this difference was statistically significant (p < 2.2e-16), suggesting the NHL trend is not merely due to more Canadians being born early in the year.

To assess whether this pattern holds across nationalities, I created a comparative bar plot of Canadian vs. Non-Canadian players. Interestingly, the early-year birth bias persisted in both groups, supporting the theory that youth development systems — not just birth distribution — play a key role.

The final set of visualizations looked at the globalization of hockey. Two pie charts showed that in the mid-1990s, Canadian players dominated the NHL. However, a line graph tracking player counts over time illustrated the league's increasing international diversity — even as the number of Canadian players continues to grow.

Lastly, a scatterplot examined physical attributes by player position. The analysis showed that:
- Goalies tend to be lighter and shorter,
- Forwards fall in the middle range,
- Defensemen are generally taller and heavier.

# EconPowerPred-G20-World-Economic-Center-Prediction
This project aims to predict the probability of each country in the G20 group to become the World Economic Center in the future. The G20 group consists of 19 countries and the European Union, which together account for more than 80% of the global GDP, trade, and population. The G20 group is considered the most influential and representative forum for international economic cooperation and decision-making.

## Data Sources and Factors
The project utilizes 12 datasets from various sources that reflect different aspects of economic development and performance. These factors include:-

* Coal Production
* Crude Oil Production
* Ease of Doing Business
* Employment Rate
* GDP per capita
* Global Innovation Index
* Global Knowledge Index
* Health Expenditure
* Infrastructure Score
* Political Stability
* Quality of Life
* Working Age Population

The datasets cover the period from 2000 to 2020 for each country in the G20 group

## Analysis and Prediction
The project consists of two Jupyter notebooks: *Analysis.ipynb* and *Prediction.ipynb*. 

In **Analysis.ipynb**, the project explores and visualizes the data for each factor and country using bar plots and time series plots. These plots showcase the trends and patterns of each factor over time and across countries.

In **Prediction.ipynb**, the project applies a ranking-based approach to predict the probability of each country becoming the World Economic Center. The steps involved are as follows:
1.	For each factor, rank the countries according to their scores, with lower rank indicating higher impact in that respective considered factor.
2.	For each country, calculate the average rank across all factors. For example, India has rankings of 3,11,15,17,20,15,19,16,16,18,15,11 respectively for all factors. Then India has an average rank of 14.667.
3.	For each country, calculate the adjusted rank by subtracting the average rank from 20 (the maximum possible rank). For example, India has an adjusted rank of 20 - 14.667 = 5.333.
4.	For each country, calculate the probability by dividing the adjusted rank by the sum of all adjusted ranks and multiplying by 100. For example, India has a probability of 5.333 / 201.333 * 100 = 2.673%.

The final probabilities are shown in the table below in descending order:
| Country |  Probability (%)  |
|:-----|:--------:|
| United States   | 7.979 |
| Canada   |  7.520  |
| Australia   | 7.436 |
| Germany   | 6.935 |
| United Kingdom   | 6.684 |
| European Union   | 6.266 |
| Japan   | 5.932 |
| France   | 5.305 |
| China   | 5.196 |
| South Korea|5.013|
|Saudi Arabia|	5.172
|Russia|	4.967
|Italy|	4.470
|Brazil|	3.300
|Argentina|	3.196
|Mexico|	3.468
|Turkey|	3.008
|South Africa|	2.882
|India|	2.673
|Indonesia|	2.598|

## Conclusion
The project provides a simple and intuitive way to compare and predict the economic potential of different countries in the G20 group based on multiple factors. The results show that the United States, Canada, Australia, Germany and the United Kingdom have the highest probabilities to become the World Economic Center, while Indonesia, India, South Africa, Turkey and Mexico have the lowest probabilities.

The high probabilities of the top five countries reflect their strong performance in various aspects of economic development, such as innovation, infrastructure, quality of life and political stability. These countries also have high GDP per capita and health expenditure, which indicate their wealth and well-being. Moreover, these countries have relatively low coal and crude oil production, which suggest their lower dependence on fossil fuels and their transition to cleaner and more sustainable energy sources.

The low probabilities of the bottom five countries indicate their challenges and weaknesses in achieving economic growth and competitiveness. These countries have low scores in ease of doing business, global innovation index and global knowledge index, which imply their difficulties in creating a conducive environment for entrepreneurship, research and education. These countries also have high coal and crude oil production, which imply their reliance on non-renewable and polluting energy sources. Furthermore, these countries have low quality of life and political stability, which affect their social and institutional stability and security.

## Possible Future Challenge

__External Validation__: 
Check if my predictions match with what happens in the real world. This could include watching global economic trends, changes in politics, or big decisions and seeing how well this predictions agree with these real-world results.

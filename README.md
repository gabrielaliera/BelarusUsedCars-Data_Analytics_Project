# BelarusUsedCars-Data_Analytics_Project

<p align="center">
  <img align="center" src="https://github.com/gabrielaliera/BelarusUsedCars-Data_Analytics_Project/blob/e394cc2da67cdbb1113c278a07541b56cfe22abb/pictures/belarus%20map2.jfif">
</p>

# Project Information
This project is based on a dataset of a 2019 online catalog for used cars market in Belarus (eastern Europe). The dataset contains data that was parsed from car ads in an online catalog. This dataset is useful for both the buyer and the seller in the used car market in Belarus. Our dataset is from <a href="https://www.kaggle.com/lepchenkov/usedcarscatalog">Kaggle</a>. 

# Questions
1. Which region has the highest number of cars listed in the online catalog?
2. In this region, which car brands and models have the highest listing in the catalog?
3. Which body type and color has the highest listing?
4. Which transmission, fuel type, and drive-wheel has the highest listing?
5. What are the average prices per body type?
6. What is the range of the price and the age of the cars listed?
7. Is there a correlation between the age of car and price?
8. Do expensive cars have more number of photos?
9. Does having more photos lead to more views?
10. If the number of views increase, do the number of days listed decrease?
11. Is there a relationship between the type of transmission and the price of the car?
12. Are the diesel car prices significantly higher or lower than the gasoline car prices?
13. Are transmission and fuel types independent or dependent?
  
# Sample Code

### Sample 1
<p align="center">
  <img align="center" src="https://github.com/gabrielaliera/BelarusUsedCars-Data_Analytics_Project/blob/main/pictures/samplecode_function.PNG">
</p>

### Sample 2
<p align="center">
  <img align="center" src="https://github.com/gabrielaliera/BelarusUsedCars-Data_Analytics_Project/blob/main/pictures/samplecode_pivot2.PNG">
</p>


# Sample Data Visualizations

### Data Visualization Sample 1
<p align="center">
  <img align="center" src="https://github.com/gabrielaliera/BelarusUsedCars-Data_Analytics_Project/blob/main/pictures/samplecode.PNG">
</p>
<p align="center">
  <img align="center" src="https://github.com/gabrielaliera/BelarusUsedCars-Data_Analytics_Project/blob/main/pictures/samplecode_visualization.PNG">
</p>

### Data Visualization Sample 2
<p align="center">
  <img align="center" src="https://github.com/gabrielaliera/BelarusUsedCars-Data_Analytics_Project/blob/main/pictures/linear_relationship.PNG">
</p>

# Sample Statistical Test
<p align="center">
  <img align="center" src="https://github.com/gabrielaliera/BelarusUsedCars-Data_Analytics_Project/blob/main/pictures/chi-square-test2.PNG">
</p>
<p align="center">
  <img align="center" src="https://github.com/gabrielaliera/BelarusUsedCars-Data_Analytics_Project/blob/main/pictures/chi-square-results.PNG">
</p>


# Tech/Framework
<ul>
  <li><a href="https://www.python.org/">Python</a></li>
  <li><a href="https://jupyter.org/">Jupyter Notebooks</a></li>
  <li><a href="https://www.kaggle.com/">Kaggle</a></li>
  <li><a href="https://numpy.org/">NumPy</a></li>
  <li><a href="https://pandas.pydata.org/">Pandas</a></li>
  <li><a href="https://matplotlib.org/">Matplotlib</a></li>
  <li><a href="https://seaborn.pydata.org/">Seaborn</a></li>
  <li><a href="https://scipy.org/">SciPy</a></li>
  <li><a href="https://www.statsmodels.org/stable/index.html">Statsmodel</a></li>
  
</ul>

#  Exploratory Data Analysis Findings

This original data set included over 30,000 records. However, we wanted to focus on the Minsk region of Belarus because it had two-thirds of the cars listed in the catalog. Within the Minsk region, Volkswagen had the highest number of cars listed. Therefore we decided to conduct a deep analysis on used Volkswagen cars in Minsk.

## 1. Which region has the highest number of cars listed in the online catalog?

Minsk, which is the capital of Belarus, has the highest number of cars.

## 2. In this region, which car brands and models have the highest listing in the catalog?

The top brand in Minsk is Volkswagen, followed by BMW, Opel, Ford, and Renault. Therefore, we focused our study on Volkswagen whose most common models found in the listing are Passat, Golf, Touran, Jetta, T4, Polo Sedan, Sharan, Polo, Touareg, and Tiguan. Passat comprise about 36% of the listings of Volkawagen followed by Golf (~21%).

## 3. Which body type and color has the highest listing?

Sedan has the highest listing for body type followed by universal, and hatchback. The color black has the highest listing followed by silver and blue.

## 4. Which transmission, fuel type, and drive-wheel has the highest listing?

The top listing in:
<ul>
  <li>Transmission - Mechanical</li>
  <li>Fuel Type - Gasoline</li>
  <li>Drive-Wheel - Front Wheel</li>
</ul>


## 5. What are the average prices per body type?

We observe that Sedans and Universals have the highest listing in the catalog, however, their average prices are much lower than the SUVs, which have the highest average price. SUVs and Minibus body type has more outliers that are higher in price.

When comparing fuel types, diesel cars have a higher price than gasoline cars. We will explore this in our hypothesis.

Used cars with automatic transmission generally have a higher average price than the used cars with mechanical transmission. SUVs and Minibus with automatic transmission are more expensive than rest of the cars. Sedans and Universal cars have similar price range for both automatic and mechanical transmission type.

## 6. What is the range of the price and the age of the cars listed?

The darkest region of a jointplot shows that majority of the cars are between 7 and 15 years old with prices ranging from 5000 USD to 8000 USD. The second highest density range is from 20 to 30 years old with price ranging between 1000 USD t0 4000 USD.

## 7. Is there a correlation between the age of car and price?

As the age of the car increases, the price decreases. However, there is a very weak correlation between them as shown in our regplot.

## 8. Do expensive cars have more number of photos?

Expensive cars do not necessarily have more photos posted online. Having a high number of photos also does not lead to an increase in price. There is strong evidence that the linear correlation is weak as shown in our regplot.

## 9. Does having more photos lead to more views?

There is no correlation between the numbers of photos and the number of views. There could be other factors that lead to more views.

## 10. If the number of views increase, does the number of days listed decrease?

As the number of days listed increases, the number of views increases. It may be the car has been listed longer so it has a higher number of views. Our analysis shows that there is weak evidence of the correlation between these 2 factors.

## 11. Is there a relationship between the type of trasmission and the price of the car?

The prices between Automatic and Mechanical Transmission are significantly different based on our ANOVA test.

## 12. Are the diesel car prices significiantly higher or lower than the gasoline car prices?

The average diesel car prices are significantly greater than the average of gasoline car prices.

## 13. Are transmission and fuel types independent or dependent?

Based on a Chi-Square test for independence, transmission and fuel type are probably dependent.

# Contributors
  <ul>
  <li>Gabriela Liera</li>
  <li>Geeta Ganesh</li>
  <li>Gargi Misra</li>
  </ul>

# Notes
View the entire project- <a href="https://github.com/gabrielaliera/BelarusUsedCars-Data_Analytics_Project/blob/main/CISD41_Project_3Gs_Belarus_Used_Cars.ipynb">Belarus Used Cars</a> 

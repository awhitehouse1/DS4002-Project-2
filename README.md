# Contents of Repository 
# Section 1: Software and Platforms
All of our code was written in Python using Google Colab's notebooks. Google Colab made sharing code simpler and allowed us to work on both Windows and Mac machines without any issues.
For add-on packages, pandas was used for data processing and manipulation. Matplotlib and seaborn were used for creating visualizations. The statsmodels module was used to create the ARIMA and ARIMAX models.

# Section 2: Map of documentation
In our repository, there are folders for the data, scripts, and output. The original data sources from Data World, The World Bank Group, and Our World in Data are located in the data folder.
- In the Data folder:
  - democracy-index-eiu.csv: Original data source for democracy index scores
  - gdp_per_capita.csv: Original data source for GDP per capita
  - obtaining_covid_data.pdf: Contains link and instructions for downloading the original data source for the COVID-19 time series data
  - NEW_time_series_data.csv: Processed and cleaned data that includes the number of deaths per million per day, from 1/22/2020 to 1/22/2022, by country. It also includes the GDP per capita and democracy score for each country on the particular day.
  - DataAppendix.pdf: includes tables, figures, and other descriptive statistics about the data
- In the Scripts folder:
  - Final_Cleaning.ipynb: Code used to clean and merge our input data into our analysis file 'NEW_time_series_data.csv'
  - Final_EDA.ipynb: Code used for exploratory data analysis
  - VAR.ipynb: Code used to run our Vector Autoregression model
  - ARIMA_(X)_Analysis.ipynb: Code used to run our ARIMA and ARIMAX models
- In the Output folder:
  - ARIMAX_UnitedStates_covid_gdp_democracyScore.png: includes a plot of the ARIMAX forecast for the United States
  - ARIMAX_error_metrics_table.png: includes error metrics for our ARIMAX model, such as mean absolute error and mean squared error
  - ARIMA_by_country.pdf: includes plots of the ARIMA model forecasts for all 20 countries used in our analysis

# Section 3: Instructions for reproducing our results
1. Navigate to the Scripts folder of our repository, where you will see multiple Python notebook scripts.
2. Download the VAR.ipynb file. This is the file needed to run the VAR model. 
3. Download the ARIMA_(X)_Analysis.ipynb file. This is the file needed to run the ARIMA and ARIMAX models after the VAR model. 
4. Navigate to the Data folder of our repository and download the NEW_time_series_data.csv file. Then click on the obtaining_covid_data pdf and follow the instructions to download the COVID-19 time series data. This is the data that is needed to run the code. 
6. Upload these files to Google Colab (https://colab.research.google.com/). This is where the code will be run.
7. Open the VAR.ipynb file in Colab. Make sure that the filepaths for the datasets, located at the beginning of the file, are where you have the code stored on your local machined. Run the code by selecting "Runtime -> Run All" in the Colab tool menu. This will install all of the needed packages and then implement the VAR model.
8. Next, open the ARIMA_(X)_Analysis.ipynb file to run the final part of the analysis. 

# References
https://machinelearningmastery.com/arima-for-time-series-forecasting-with-python/
https://www.analyticsvidhya.com/blog/2021/08/vector-autoregressive-model-in-python/
https://www.analyticsvidhya.com/blog/2021/06/statistical-tests-to-check-stationarity-in-time-series-part-1/#:~:text=There%20are%20various%20statistical%20tests,unit%20root%20in%20the%20data. 

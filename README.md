# Contents of Repository 
# Section 1: Software and Platforms
All of our code was written in Python using Google Colab's notebooks. Google Colab made sharing code simpler and allowed us to work on both Windows and Mac machines without any issues.
For add-on packages, pandas was used for data processing and manipulation. Matplotlib and seaborn were used for creating visualizations.

# Section 2: Map of documentation
In our repository, there are folders for the data, scripts, and output. The original data sources from Data World, The World Bank Group, and Our World in Data are located in the data folder.
- In the Data folder:
  - democracy-index-eiu.csv: Original data source for democracy index scores
  - gdp_per_capita.csv: Original data source for GDP per capita
  - NEW_time_series_data.csv: Processed and cleaned data that includes the number of deaths per million per day, from 1/22/2020 to 1/22/2022, by country. It also includes the GDP per capita and democracy score for each country on the particular day.
  - DataAppendix.pdf: includes tables, figures, and other descriptive statistics about the data
- In the Scripts folder:
  - Final_Cleaning.ipynb: code used to clean and merge our input data into our analysis file 'NEW_time_series_data.csv'
  - Final_EDA.ipynb: code used for exploratory data analysis
  - Testing_country_code.ipynb: code used to run our VAR and SARIMAX time series models
- In the Output folder:

# Section 3: Instructions for reproducing our results
1. Navigate to the Scripts folder of our repository, where you will see multiple Python notebook scripts.
2. Download the Testing_country_code.ipynb file. This is the file neede to run the VAR and SARIMAX models.
3. Download the ____ file. This is the file needed to run the hypothesis testing.
4. Navigate to the Data folder of our repository and download the NEW_time_series_data.csv file. This is the data that is needed to run the code.
5. Upload these files to Google Colab (https://colab.research.google.com/). This is where the code will be run.
6. Open the ___ file in Colab. Run the code by selecting "Runtime -> Run All" in the Colab tool menu. This will install all of the needed packages, clean the data, and then implement ___.
7. Open and run the code in the ___ (hypothesis testin) file.

# References
https://www.analyticsvidhya.com/blog/2021/08/vector-autoregressive-model-in-python/
https://www.analyticsvidhya.com/blog/2021/06/statistical-tests-to-check-stationarity-in-time-series-part-1/#:~:text=There%20are%20various%20statistical%20tests,unit%20root%20in%20the%20data. 

# uep239-finalproject
# Final project for Geospatial Programming with Python (Tufts University)

**Summary:**  For my vulnerability analysis, I will be determining which zipcodes in Massachusetts would be most vulnerable in the event of a natural disaster. This is based on 5 indicators: 
1. Percentage of elderly residents (65 years and older) in each zipcode
2. Percentage of residents in each zipcode who earn less than $35,000 USD annually
3.Percentage of people in each zipcode who were not born in the United States
4. Percentage of households in each zipcode that speak limited English
5. Euclidean distances of hospitals in each zipcode

This notebook can be run by cloning the repository from GitHub and running each cell in the notebook.

**Data Files**
ACSST5Y2019.S0101 - Contains demographic data for people living in Massachusetts, such as age and sex, for each zipcode within the state.

ACSST5Y2019.S0501_2021-05-12T161803 - Contains data for people living in the state of Massachusetts who were born outside of the United States, based on zipcode. 

ACSST5Y2019.S1602_2021-05-12T065118 - Contains data for people living in the state of Massachusetts who speak limited English.

ACSST5Y2019.S2503 -  Contains financial data for people living in the state of Massachusetts

HOSPITALS_PT- Contains data on hospitals in the state of Massachusetts.

tl_2010_25_zcta510 - Contains data on zipcodes in the state of Massachusetts. 

**Preprocessing Steps**
1. Changed the column names in the tabular indicator data. 
2. Also, removed 'ZCTA ' from each of the zipcode values in tabular indicator data so that they could be merged to the zipcode data.
3. From tabular indicator data, selected the columns that were going to be focused on. 

**Packages Used**
pandas 
matplotlib.image 
%matplotlib inline
folium   
seaborn 
geopandas 
rasterio 
rasterio.plot 
affine 
math
scipy
rasterstats
numpy 
matplotlib.pyplot

**Sites Used:** 
*Removing unwanted parts from strings in a column: *https://stackoverflow.com/questions/13682044/remove-unwanted-parts-from-strings-in-a-column 

*Data Normalisation:* https://towardsdatascience.com/data-normalization-with-pandas-and-scikit-learn-7c1cc6ed6475

https://pandas.pydata.org/pandas-
docs/stable/reference/api/pandas.DataFrame.count.html

*Calculating Euclidean distance:* https://docs.scipy.org/doc/scipy/reference/generated/scipy.ndimage.distance_transform_edt.html

*Choropleth map info:* https://towardsdatascience.com/lets-make-a-map-using-geopandas-pandas-and-matplotlib-to-make-a-chloropleth-map-dddc31c1983d

*Aggregation:* https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.agg.html

*Merging Dataframes:* https://geopandas.org/docs/user_guide/mergingdata.html
https://gis.stackexchange.com/questions/349244/merging-a-geodataframe-and-pandas-dataframe-based-on-a-column

*Mean:* https://www.kite.com/python/answers/how-to-find-the-mean-of-a-pandas-dataframe-column-in-python#:~:text=Use%20pandas.,mean%20of%20a%20DataFrame%20column

**Acknowledgements**

Huge thank you to all the instructors of UEP239. Literally could not have done this without you all. 





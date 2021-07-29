# Chicago E-Coli Test Results
This project consists of an analysis of the E. coli levels of the Chicago beaches. Data was gathed via public data from the City of Chicago, through CSV files, in addition to APIs to access certain weather data. Beach data is found at https://data.cityofchicago.org/Parks-Recreation/Beach-Lab-Data/2ivx-z93u. 

Data was collected via two methods. The first, and more established method, is a cell culture based method, which is an established (used by the EPA), but rather slow (results take 24-48 hours) method. This method was predominantly used from 2006 until 2016. Additionally, a new method was used to also collect data, using qPCR, a DNA analysis technique. This method provides more rapid results (4-6 hours) and has been used more predominantly since 2016, and is used currently. 

![Culture by Month](https://github.com/ander1908/Bootcamp_Project1/blob/main/output/Culture_Days_Exceeing_Threshold_by_Month.png)
![DNA by Month](https://github.com/ander1908/Bootcamp_Project1/blob/main/output/DNA_Days_Exceeing_Threshold_by_Month.png)

The aim of the project was to identify any trends or relationships of interest that may be present, and to determine the freuency and intensity of days exceeding health and safety standards. 

![Culture Threshold](https://github.com/ander1908/Bootcamp_Project1/blob/main/output/Culture_Readings_Above_Threshold_by_Month.png)
![DNA Threshold](https://github.com/ander1908/Bootcamp_Project1/blob/main/output/DNA_Readings_Above_Threshold_by_Month.png)

Data was cleaned and analyzed using Pandas, through Jupyter Notebook. Additionally, using Matplotlib, visualizations of the data and relevant finds were displayed. Also, Gmaps was used to create a heatmap to visualize the severity of the E. coli levels at the beaches. 

Furthermore, it is known that Milwaukee releases sewage into Lake Michigan during periods of high rainfall and other situations where the system is overwhelmed. Our group wanted to investigate whether a relationship existed between the level of Milwaukee rainfall and the levels of E. coli in the chicago beaches. This was accomplished using a weather API, https://www.worldweatheronline.com/developer/. 

The code in this repository consists of a variety of CSV files that were created throughout the data cleaning and the analysis portions. The various group members created CSVs for ease of use, as other group members sometimes required their previous analysis and built on top of them.

The data cleaning code is found in "Data_Cleaning.ipynb". The analysis has been consolidated into "Final Data Analysis.ipynb". However, the weather API data was kept separate, and is found in the "Milwaukee_Historical_Weather_Data_API_Calls.ipynb" file.

There are additional Jupyter Notebooks in this repository that contains the analysis separated by the group member's work. 

Lastly, figures of all of the plots generated during this analysis can be found in the "output" directory. 

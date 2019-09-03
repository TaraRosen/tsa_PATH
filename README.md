# Data Science Module 6 Project 
* Gordon Chen & Tara Rosen(nyc-mhtn-ds-0422019)
* Flatiron School

## Project Description
The Module 6 Project of the Flatiorn Data Science program was to create a prediction model using Time Series Analysis methods. This project focuses on using monthly Path train ridership data to predict future trends in ridership. The Time Series model that we ended up using was SARIMA model from Statsmodel. We used Mean Absolute Percentage Error as a performance measure for the Time Series model.

## Project Background
The PATH is a mass transit system that connects New Jersey and New York. There are currently 4 lines with 13 station stops:

![path_map](https://github.com/TaraRosen/ts_analysis_PATH/blob/master/Images/slide_8.png)

Presently, Jersey City, NJ is experiencing a growth spurt and in the midst of adding 66,000 residential units to the city. Of the 7 New Jersey PATH stations, 4 of them are in Jersey City and the majority of these new residential units are within walking distance of these PATH staions. As a resident of Jersey City and a frequent PATH commuter, all of this new construction piqued my interest on current PATH ridership and where it may be heading into the future. 

PATH History

* Built in 1908 for a maximum monthly ridership of 7.5 million
* In 2018 the average monthly ridership was 6.5 million 
* In August, 2017, the PATH hit a maximum ridership of 7.7 million

It appears that the PATH system is approaching its design capacity.

Our Approach

* We created a PATH Monthly Ridership dataset

![ridership](https://github.com/TaraRosen/ts_analysis_PATH/blob/master/Images/slide_3.png)

* Optimized Parameters

    - AR(p)
    - I(d)
    - MA(q)
    - S(s)
    - P
    - D
    - Q
    
![para_opt](https://github.com/TaraRosen/ts_analysis_PATH/blob/master/Images/slide_4.png)
    

* Trained the SARIMA (Seasonal Autoregressive Integrated Moving Average) Model


![training](https://github.com/TaraRosen/ts_analysis_PATH/blob/master/Images/slide_5.png)


* Forecasted Future Ridership Using SARIMA Model


![future](https://github.com/TaraRosen/ts_analysis_PATH/blob/master/Images/slide_6.png)
    


### Data Sources
#### Path NY NJ
PATH Ridership Report (by month)
https://www.panynj.gov/path/statistics.html

#### Data.gov
Port Authority Trans-Hudson (PATH) Monthly Ridership: Beginning 1996
https://catalog.data.gov/dataset/port-authority-trans-hudson-path-monthly-ridership-beginning-1996


### Deliverables
#### Jupyter Notebooks
* [Final_NJ_Path.ipynb] This notebook contains the details of Time Series Analysis performed on the dataset and the ridership forecasting


### Conclusion and Presentation
* https://docs.google.com/presentation/d/1MbBbslcKVdNShHIfutHsTh--khCSl0aS1IUaARWDIts/edit?usp=sharing
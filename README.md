## Air_Quality_Index_Prediction
Provided with the data collected from [here](https://en.tutiempo.net/climate/01-2013/ws-432950.html) from the year 2013 to 2018 and our job is to design a efficient machine learning model which given the features extracted from the collected data can predict air quality (PM2.5) value.

To determine air quality in an area, pollutant concentrations are physically measured and reported. The AQI is calculated based on the average concentration of a particular pollutant measured over a standard time interval (24 hours for most pollutants, 8 hours for carbon monoxide and ozone). For example, the AQI for PM2.5 is based on 24-hour average concentration and computed as shown in the table below:

| Category        | AQI           | 24 hour Average PM2.5 concentration (microgram/m^3)|
| ------------- |:-------------:| -----:|
| Good      | 0-50 | 0-30 |
| Satisfactory      | 51-100      |   30-60 |
| Moderate | 101-200      |   60-90 |
| Poor      | 201-300 | 90-120 |
| Very Poor      | 301-400      |   120-250 |
| Severe | 401-500      |   250-380 |

As the table shows, the AQI for PM2.5 is in the ‘good’ category (0-50) if the 24-hour average is within 0-30 microgram/m3; e.g. if the 24-hour average concentration is 15 microgram/m3, the corresponding AQI is 25.

It is severe (400+) if 24-hour averages are greater than 250 microgram/m3, and if concentrations are 380 microgram/m3 or more, they get reported as 500, the maximum possible.

### Dataset Description:
Our dataset contains 8 features (Independent Variables) and 1 dependent variable (PM2.5):
T : Average Temperature (°C)

TM : Maximum temperature (°C)

Tm :Minimum temperature (°C)

SLP :Atmospheric pressure at sea level (hPa)

H :Average relative humidity (%)

VV :Average visibility (Km)

V :Average wind speed (Km/h)

VM :Maximum sustained wind speed (Km/h)

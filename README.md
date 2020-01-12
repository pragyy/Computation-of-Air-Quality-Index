# Computation-of-Air-Quality-Index
In this project we are calculating the air quality index of Delhi.

The dataset used is a time-series data.
The dataset under consideration consists of four main pollutants viz, NO2, SO2, SPM and RSPM using which the Air Quality Index is calculated.
It contains daily concentrations of the aforementioned pollutants from 2008-2010.


The Air Quality Index was computed as follows:

There are primarily three steps involved in the calculation of AQI:
Firstly, the air pollution index for each pollutant (Q) is calculated. In this step, the concentration value of the pollutants is related to the Indian air quality standards and then the concentration of each pollutant is converted into a percentage of each standard. Then the pollution index of each pollutant is obtained.
Pollution indices are obtained by using the following formula:
 
Qi = (Ci * Si)/100
where Qi is the air pollution index for the pollutant “i”, Ci is the corresponding concentration of the pollutant “i” in the air (calculated from the dataset) and Si is the air quality standard for the pollutant as prescribed by the Indian Pollution Control Association (IPCA).
 
 
Secondly, the weighted mass (w) for each pollutant is computed.  
wi = Wi/ΣWi
where Wi is the mass of pollutant “i” 
 
 
Finally, the AQI is then calculated as follows:
AQI = Σ(Wi * Qi)

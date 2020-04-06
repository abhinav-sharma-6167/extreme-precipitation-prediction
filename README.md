
# Extreme-Precipitation-Prediction
Precipitation nowcasting at very short lead times is a difficult and important earth science goal. The implications of nowcasting extend into aviation, flood forecasting and other areas. Using correlation analysis for the generation of velocity vectors to advect a composite radar rainfall field is the method of nowcasting utilized in this work. The MIT Lincoln Laboratory Growth and Decay Storm Tracker (GDST) is a correlation-based nowcasting algorithm that utilizes spatial filtering to eliminate the potentially adverse effects of transient, small-scale rainfall features in the correlation step.
     
The GDST is used in this work to evaluate the benefits of image filtering as compared to a situation where the filtering is absent. The GDST generates a spatially variable velocity field for input rainfall field advection. Forecasts made using this enhancement are compared to forecasts made using a single velocity value for all input pixels in order to determine the benefits of allowing for differential motion within the storm envelope. The results from three storm cases show that image filtering provides improvement in forecast accuracy over an unfiltered case however, to fully determine any benefits from using spatially variable velocities requires more work.

### Work Pertaining to Study of Research Papers :
#### Extrapolation vs Machine Learning :
Objective short-term forecasting can take many forms, one of which is nowcasting. Nowcasting is defined as very short-term weather forecasting with forecast lead times ranging from zero to six hours and includes methods such as extrapolation and numerical weather prediction.

#### Disadvantage of Extrapolation method :
The accuracy of prediction decreases very quickly due to the transient nature of the atmosphere and a very large amount of factors causing changes in wind speed, humidity which in turn affect precipitation.

#### Disadvantage of Numerical Weather Prediction method :
For many applications, including hydro-meteorologic forecasting and aviation, the forecast resolutions provided by NWP models do not meet the user requirements for several reasons. The spatial resolution (30-100 km) of NWP model outputs is often so large that it misses the prediction required for a smaller sub-grid.


#### The Automated Precipitation Extrapolator (APEX)
The Automated Precipitation Extrapolator (APEX) nowcasting method was developed at the Massachusetts Institute of Technology to produce short-term nowcasts from composite radar rainfall fields. 
	The effect that current weather conditions have on weather conditions in the near future cemented the importance of extrapolation methods to overall forecasting ability. The most accurate forecasts for short lead-times (zero to six hours), when considering
mesoscale and synoptic scale NWP models and extrapolation techniques, are generated by extrapolation methods (Browning, 1980). This conclusion along with the new TREC algorithm spurred new research into other methods of nowcasting that may aid in the increase in accuracy of the forecasts.To this point, extrapolation based nowcasting methods had been con_ned to experiments using data from a single radar, not utilizing the forecasting potential provided
by regional radar networks. Many mesoscale storms have lifetimes exceeding their time in the observation area of a single radar. Advancements in data assimilation techniques and an increase in computation time helped to overcome this limitation
by allowing for the creation of regional radar mosaics.


#### APEX Algorithm Description

APEX, like other extrapolation forecasting algorithms uses a steady state assumption as its theoretical base. Applied to rainfall forecasting, this assumption implies that rainfall intensities and spatial patterns will remain the same over short forecasting
intervals. By applying a static velocity field to this static rainfall field, linear forecasts are created via a process termed “Lagrangian Persistence" since the rainfall field is persisted in a Lagrangian coordinate system (Germann and Zawadzki 2002).

This differs from “Eulerian Persistence", in which the rainfall field is persisted in a stationary frame of reference. Eulerian Persistence will be used as a basis for comparison for the Lagrangian Persistence method presented here.This algorithm is governed by a set of parameters read into the model from an external text file. These parameters control many aspects of the execution of the code, including the size of the spatial filter, several thresholds and the range in which
to search for a maximum correlation coeffcient.


#### Takeaways from BTech Thesis project under Dr. Pabitra Mitra and Dr. Sudeshna, Head of Department, Computer Science and Engineering at IIT Kharagpur  on extreme precipitation forecasting using Doppler radar image contributed valuable learnings towards convergence of our research on the same published in the International Symposium on Neural Networks (ISBN : 978-3-319-59081-3) 

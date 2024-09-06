# Enhancing Carbon Emission Reduction Strategies using OCO and ICOS data
This collection of notebooks contains the data matching, merging, trainging and visualizations used in the paper.

The notebooks should be run in numerical order, each dealing with a specific part of the process.

## 1_Format_Data.ipynb
~3 min
This notebook formats the ICOS and OCO datasets such that they use the same name for common features

## 2_Match_ICOS.ipynb
~40 min
This notebook matches each OCO observation to it's closest ICOS observation in space and time and records the distance to that station.

## ## 3_Merge_ERA5.ipynb
~3 hours
Each OCO-ICOS pair is matched to the closest ERA5 weather observation.

## 4_Train_Model.ipynb
~ The four models from the paper are trained on the full ICOS-OCO-ERA5 dataset and their accuracies are compared.

## 5_Visualizations.ipynb
This script contains additional visualizations used in the paper.

## 6_Experimental_Predictions.ipynb
This experimental notebook contains the regional predictions and interpolations used to predict ground-level CO2 outside of ICOS stations.



The data used for the analysis is not supplied in this repository. Required Data:
OCO2 observations: data/raw/OCO2_Europe_good_data.csv
ICOS CO2 measurements: data/raw/ICOS_CO2_weather_euOct282023.csv
Monthly weather data from ERA5: data/raw/era5/era5_[year]_[month]_Europe.nc
Optionally, Swedish RegSO border polygons for regional prediction []: data/RegSO_2018_v2.gpkg

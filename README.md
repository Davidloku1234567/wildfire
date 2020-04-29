# Analysis of wildfire in California
### Table of Contents
1. [Installations](#installations)
2. [Project Motivation](#project_motivation)
3. [File Descriptions](#file_descriptions)
4. [Results](#results)
5. [Licensing, Authors, Acknowledgements](#licensing)

### Installations<a name="installations"></a>
Standard libraries installed with the Anaconda distribution.

python 3.7.4

### Project Motivation<a name="project_motivation"></a>

Exploratory data analysis of wildfire in California

1. What are the most and least fire-prone counties in California? 

2. What is the distribution of stated causes of fire in California? 

3. One versus the rest classification for predicting stated cause of fire


### File Descriptions<a name="file_descriptions"></a>

wildFire_1.ipynb: Jupyter notebook for EDA of wildfires in California

LICENSE.txt: MIT License

### Results<a name="resluts"></a>

The dataset includes 1.88 million geo-referenced U.S. wildfire records from 1992 to 2015. It is downloaded from kaggle. 
There are 27 tables, and the data from the table 'Fires' is used for this analysis. 

Ten most fire-prone counties in California are Riverside, Los Angeles, El Dorado, San Bernardino, San Diego, Fresno, Siskiyou, Shasta, Butte, and Kern. 

Ten least fire-prone counties in California are San Benito,
 Solano,
 Ventura,
 Kings,
 Colusa,
 Glenn,
 Marin,
 Sutter,
 San Francisco, and 
 Douglas. 
  
The five most frequent stated causes of fire in California is Miscellaneous, Equipment Use, Lightning, Arson, and Debris Burning. 

The dataset for wildfire in California initially contained thirteen features. The features 'COUNTY', and 'FIPS_NAME' had about 70% of values missing, and therefore they were dropped. 
Random forest classifier from sklearn was used for one versus the rest classification to predict the stated causes of fire. 
The classes of training data was balanced by upsampling. 

The model worked best for predicting stated cause of fire, 'Lightning', with AUC of 0.98. 
However, AUC's for predicting 'Miscellaneous' and 'Equipment Use' were less than 0.75. 
The AUC's for 'Arson' and 'Debris Burning' were 0.80 and 0.83 respectively. 

### Licensing, Authors, Acknowledgements<a name="licensing"></a>

Short, Karen C. 2017. Spatial wildfire occurrence data for the United States, 1992–2015 [FPA_FOD_20170508]. 4th Edition. Fort Collins, CO: Forest Service Research Data Archive. 

https://doi.org/10.2737/RDS-2013-0009.4

https://www.kaggle.com/rtatman/188-million-us-wildfires

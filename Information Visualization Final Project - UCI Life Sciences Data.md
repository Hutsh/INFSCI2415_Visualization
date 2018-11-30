# Information Visualization Final Project - UCI Life Sciences Data

## Data description

#### Forest type mapping Data Set

Forest type mapping Dataset is from the UCI Machine Learning Repository(https://archive.ics.uci.edu/ml/datasets/Forest+type+mapping ). The source of this dataset was collected in a forested area in Ibaraki Prefecture(36◦ 57′ N, 140◦ 38′ E), Japan, where contains mainly Cryptomeria japonica (Sugi, or Japanese Cedar) planted forest, Chamaecyparis obtusa (Hinoki, or Japanese Cypress) planted forest and mixed deciduous broadleaf natural forest. The total area where the data was collected is approximately 13 km × 12 km. Data was collected by 15 m spatial resolution multispectral Advanced Spaceborne Thermal Emission and Reflection Radiometer(ASTER) and removed the effects of image perspective(tilt) and relief (terrain) effects by Orthorectification. Only the information in three bands of the images was remained in the dataset: green (0.52–0.60 μm), red (0.63–0.69 μm) and near-infrared (NIR) (0.76–0.86 μm).    `(Johnson, Tateishi, & Xie, 2012)`

This data set contains two parts: training and testing. the trainning set has 199 instances, testing data has 325 instances. Each dataset has 27 attributes. Since this is a dataset used to solve classification problems, the first column is the class of each instance: 's', 'h', 'd' and 'o', represent 'Sugi forest', 'Hinoki forest', 'Mixed deciduous' forest' and 'Other non-forest land respectively. From the second column to the tenth column(b1 to b9 ) are the ASTER image of three bands(green, red, and near infrared wavelengths) for three dates (Sept. 26, 2010; March 19, 2011; May 08, 2011).  In order to minimize classification errors, the image data was predicted by using inverse distance weighting (IDW) interpolation method. The idea of this method is that the geographic data sets has spatial autocorrelation `(O’Sullivan and Unwin 2003)`, which means that two areas that located close to each other share the similar natrure characteristics. In the dataset, column 11 to column 28 are the information created by this idea. Column 11 to 19(pred_minus_obs_S_b1 - pred_minus_obs_S_b9) are the predicted value minus actual spectral values for the 's' class(b1 -b9); column 20 to 28(pred_minus_obs_S_b1 - pred_minus_obs_S_b9) are the predicted value minus actual spectral values for the 's' class(b1 -b9); 

- List of columns:

`class`, `b1`, `b2`, `b3`, `b4`, `b5`, `b6`, `b7`, `b8`, `b9`, `pred_minus_obs_H_b1`, `pred_minus_obs_H_b2`, `pred_minus_obs_H_b3`, `pred_minus_obs_H_b4`, `pred_minus_obs_H_b5`, `pred_minus_obs_H_b6`, `pred_minus_obs_H_b7`, `pred_minus_obs_H_b8`, `pred_minus_obs_H_b9`, `pred_minus_obs_S_b1`, `pred_minus_obs_S_b2`, `pred_minus_obs_S_b3`, `pred_minus_obs_S_b4`, `pred_minus_obs_S_b5`, `pred_minus_obs_S_b6`, `pred_minus_obs_S_b7`, `pred_minus_obs_S_b8`, `pred_minus_obs_S_b9`



## Visualizations

#### Forest type mapping Data Set

- Distribution of classes

![001](/Users/hutsh/Documents/PITT/2018Fall/IV/Final/ForestTypes/imgs/001.png)

- Band values



## Observations of relationships



## Appendix

## Reference

1. Johnson, B., Tateishi, R., Xie, Z., 2012. Using geographically-weighted variables for image classification. Remote Sensing Letters, 3 (6), 491-499.
2. O' Sullivan, D., Unwin, D., 2003, Geographic Information Analysis, pp. 28–30, 197–202, 227–233 (Hoboken, NJ: Wiley)
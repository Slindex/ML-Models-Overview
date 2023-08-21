# ML Models Overview

This project is a practical knowledge recopilation for testing different ML models based on the same problematic. All models from the same category are prepared and trained with a common dataset.

Please refer to the following table for check all the files content:

| ID | Name          | Type   | Description                                                           |
|----|---------------|--------|-----------------------------------------------------------------------|
| 1  | magic04       | .data  | DataSet for Magic Gamma Telescope practice                            |
| 2  | SeoulBikeData | .csv   | DataSet for Seoul Bikes Demand practice                               |
| 3  | Supervised CM | .ipynb | Supervised Classification Models practice and overview                |
| 4  | Supervised RM | .ipynb | Supervised Regression Models practice and overview                    |

## Magic Gamma Telescope - SCM

This practice aims to predict wheter a ray caught from the **Atmospheric Cherenkov Telescope** is Gamma or Hadron classification. In the practice the following ML models were tested in order to find the most suitable solution:

* K-Nearest Neighbors
* Naive Bayes
* Log Regression
* Support Vector Machines
* Neural Network

### Attribute Information

The following table contains the summarized information about the dataset attributes used for this ML model. This attributes are also known as *Features* that will be passed into this model in order to predict a *label*, which in this case is the class column (Ray Classification).

| ID | Name    | Type       | Description                                                           |
|----|---------|------------|-----------------------------------------------------------------------|
| 1  | fLength | continuous | major axis of ellipse [mm]                                            |
| 2  | fWidth  | continuous | minor axis of ellipse [mm]                                            |
| 3  | fSize   | continuous | 10-log of sum of content of all pixels [in #phot]                     |
| 4  | fConc   | continuous | ratio of sum of two highest pixels over fSize [ratio]                 |
| 5  | fConc1  | continuous | ratio of highest pixel over fSize [ratio]                             |
| 6  | fAsym   | continuous | distance from highest pixel to center, projected onto major axis [mm] |
| 7  | fM3Long | continuous | 3rd root of third moment along major axis [mm]                        |
| 8  | fM3Trans| continuous | 3rd root of third moment along minor axis [mm]                        |
| 9  | fAlpha  | continuous | angle of major axis with vector to origin [deg]                       |
| 10 | fDist   | continuous | distance from origin to center of ellipse [mm]                        |
| 11 | class   | g,h        | gamma (signal), hadron (background)                                   |

## Seoul Bikes - SRM

This practice aims to predict the number of public bicycles rented at noon in the **Seoul Bike Sharing System**. In the practice the following ML models were tested in order to find the most suitable solution:

* Linear Regression
* Multiple Linear Regression
* Regression with Neural Network
* Neural Network

### Attribute Information

The following table contains the summarized information about the dataset attributes used for this ML model. This attributes are also known as *Features* that will be passed into this model in order to predict a *quantity*, which in this case is the bike_count column.

| ID | Name       | Type       | Description                        |
|----|------------|------------|------------------------------------|
| 1  | bike_count | discrete   | count of bikes rented at each hour |
| 2  | hour       | discrete   | hour of the day                    |
| 3  | temp       | continuous | temperature [celsius]              |
| 4  | humidity   | discrete   | humidity [ratio]                   |
| 5  | wind       | continuous | windspeed [m/s]                    |
| 6  | visibility | discrete   | 10m                                |
| 7  | dew_pt_temp| continuous | [celsius]                          |
| 8  | radiation  | continuous | [MJ/m2]                            |
| 9  | rain       | continuous | [mm]                               |
| 10 | snow       | continuous | [cm]                               |
| 11 | functional | nominal    | functional day                     |
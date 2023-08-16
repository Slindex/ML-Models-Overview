# Magic Gamma Telescope - ML Model

This model aims to predict wheter a ray caught from the **Atmospheric Cherenkov Telescope** is Gamma or Hadron classification. This is a supervised ML model.

## Attribute Information

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
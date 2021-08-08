# Streetlight CNN classification
by Gavin Wiehl,  Liam Mulcahy, and Chad Sopata.
Streetlight classification project for DS 6012. Includes CNN with transfer learning

* data gathering scripts - Scripts used to query Google Street View Static API
  * ImageMetadata_Scraping_Streetlights.ipynb - Script for scraping the image metadata
  * Image_Scraping_Streetlights.ipynb - Script for pulling in images
* Streetlights_Baseline_Model.ipynb - Baseline model on 4 classes
* Streetlights_InceptionResNetV2_TL_Model - Version 2 of ResNet transfer model. Highest scoring model (0.9401 accuracy)

Some data gathering scripts have errors shown in the jupyter notebook. This was done post hoc in order to hide certain location data, and does not imply a problem with the script.

### Brief introduction

<img src="https://github.com/wiehlgt/UVA-streetlight-final/blob/main/images/streetlight_grid.png?raw=true" width="400" height="400">

The goal of this project is to predict the class of streetlights present in the city of Charlottesville, Virginia  based on the image of a given streetlight. We worked with Code for Charlottesville in getting streetlight location and class data. We then scraped the streetlight images from the Google StreetView API by downloading the images closest to the streetlight location data (also ensuring the camera is facing the streetlight).

The final model employed transfer learning techniques with the InceptionResNet architecture with weights initially trained on imagenet data and two added Dense layers for filter extraction. This model achieved an accuracy of 0.9401.

<img src="https://github.com/wiehlgt/UVA-streetlight-final/blob/main/images/testset_grid.png?raw=true" width="600" height="600">

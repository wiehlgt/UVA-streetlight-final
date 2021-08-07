# UVA-streetlight-final
by Gavin Wiehl,  Liam Mulcahy, and Chad Sopata.
Streetlight classification project for DS 6012. Includes CNN with transfer learning

* data gathering scripts - Scripts used to query Google Street View Static API
  * ImageMetadata_Scraping_Streetlights.ipynb - Script for scraping the image metadata
  * Image_Scraping_Streetlights.ipynb - Script for pulling in images
* Streetlights_Baseline_Model.ipynb - Baseline model on 14 classes
* Streetlights_InceptionResNetV1_TL_Model - Version 1 of ResNet transfer model
* Streetlights_InceptionResNetV2_TL_Model - Version 2 of ResNet transfer model. Highest scoring model

Some scripts have errors shown in the jupyter notebook. This was done post hoc in order to hide certain location data, and does not imply a problem with the script.

![alt text](https://github.com/wiehlgt/UVA-streetlight-final/blob/main/images/streetlight_grid.png?raw=true)

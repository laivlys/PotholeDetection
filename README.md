# Pothole Detection
This project is trained on 100 images of roads that was downloaded from Google Earth Engine. 

Using the labelme application, the potholes and uneven in the images were manually labelled and used to train the model. A MaskRCNN pretrained model was used as a basis and was fine-tuned using the hand labelled dataset of potholes. 

The type of road was also manually labelled in the Python notebook which was then used to fine tune the ResNet18 model that was used as a foundation for identifying road type. The road type was categorized into 3 different categories of road: local roads, collector roads, and arterial roads. Local roads were defined as the roads that were mainly for residential areas; collector roads were the connecting roads of local roads to arterial roads; and arterial roads are identified as highways and freeways. 

The aim is to be able to identify potholes in the roads and the type of roads that have these potholes to determine which roads have been undermaintained.


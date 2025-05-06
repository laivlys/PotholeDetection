# Pothole Detection
This project proposes a pothole detection system integrated with a road type classification model, designed to assist authorities in identifying roads requiring maintenance and prioritizing those with higher traffic volume, higher safety concern, and greater susceptibility to damage.

## Methodology 

This project is trained on 100 images of roads that was downloaded from Google Earth Engine. 

Using the LabelMe application, the potholes and uneven roads in the images were manually labelled and used to train the model. A MaskRCNN pretrained model was used as a base model due to the high accuracy rate and was fine-tuned using the hand labelled dataset of potholes. 

Roads were categorized into three main categories: local roads, collector roads, and arterial roads. Local roads typically serve residential areas, accommodate lower traffic volumes, and support slower vehicle speeds. Collector roads function as intermediaries, linking local roads to arterial roads, and generally carry moderate traffic volumes. Arterial roads, including highways and major thoroughfares, are designed to handle high traffic volumes and support faster travel speeds.

The ResNet-18 architecture was employed as the foundational model and was fine tuned using the manual classification of roads in Python. 




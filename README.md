# Geospatial-Terrain-Classification_Deep-Learning
The aim of the project is to  develop a geospatial terrain identification model using satellite images . The requirements of terrain identification range  from urban planning, Network Planning, natural resource management to disaster response and military operations . 

### Data Understanding-Geospatial Data 
EuroSAT dataset is based on Sentinel-2 satellite imagery covering 13 spectral bands and consists of 10 LULC classes with a total of 27,000 labeled and geo-referenced images. Satellite image data comes as tiff image with 12 bands and different spatial resolution.For this project, will be using RGB data includes the optical R, G and B frequency bands (B2, B3, B4) encoded as JPEG images bands . These images have spatial resolution of 10m (area covered by each pixel) acquired from patches of images of U Sentinel 2 (2A and 2B) satellites.

[EuroSAT Dataset](https://zenodo.org/records/7711810#.ZD7rSezMJQL)

### Model Training and Evaluation Summary
In this project, 7 deep learning models were trained to classify terrain images with the aim of achieving high accuracy.<br> 
The project began with a Baseline CNN Model featuring a single Max Pooling layer and one Dense layer, achieving an initial test accuracy of 73.4%. <br>
Subsequent models were developed, including a Simple CNN Model with additional Dense layers and regularization techniques such as L1 and L2 regularization, as well as dropout layers. While Model 1 of this approach with L1 regularization achieved only 26.5% accuracy, Model 2 significantly improved to 71%. <br>
A Deep CNN Model with three Max Pooling layers and Dense layers supplemented by dropout achieved a notable accuracy of 81%. <br>
Transfer Learning was explored using pre-trained models VGG19 and VGG16, resulting in accuracies of 80.6% and 89.4%, respectively. <br>
The final model, which involved fine-tuning VGG16 and incorporating three Dense layers with dropout, exhibited the highest accuracy of 91.1%. <br>
These results underscore the effectiveness of deep learning techniques in classifying geospatial terrain imagery.






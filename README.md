# Geospatial-Terrain-Classification_Deep-Learning
The aim of the project is to  develop a geospatial terrain identification model using satellite images . The requirements of terrain identification range  from urban planning, Network Planning, natural resource management to disaster response and military operations . 

### Data Understanding-Geospatial Data 
EuroSAT dataset is based on Sentinel-2 satellite imagery covering 13 spectral bands and consists of 10 LULC classes with a total of 27,000 labeled and geo-referenced images. Satellite image data comes as tiff image with 12 bands and different spatial resolution.For this project, will be using RGB data includes the optical R, G and B frequency bands (B2, B3, B4) encoded as JPEG images bands . These images have spatial resolution of 10m (area covered by each pixel) acquired from patches of images of U Sentinel 2 (2A and 2B) satellites.

[EuroSAT Dataset](https://zenodo.org/records/7711810#.ZD7rSezMJQL)

### Models Trained

1. **Baseline CNN Model**

   - **Architecture:** Convolutional Neural Network with 1 Max Pooling layer and 1 Dense layer.
   - **Test Accuracy:** 73.4%

2. **Simple CNN Model**

   - **Architecture:** Convolutional Neural Network with 1 Max Pooling layer and 2 Dense layers.
   - **Regularization:** Model 1: L1 Regularization, Model 2: L2 Regularization + Dropout.
   - **Test Accuracy:** Model 1: 26.5%, Model 2: 71%

3. **Deep CNN Model**

   - **Architecture:** Convolutional Neural Network with 3 Max Pooling layers and 3 Dense layers with Dropout.
   - **Test Accuracy:** 81%

4. **Transfer Learning: VGG19**

   - **Architecture:** Transfer Learning using VGG19 pre-trained model with 2 Dense layers and Dropout.
   - **Test Accuracy:** 80.6%

5. **Transfer Learning: VGG16**

   - **Architecture:** Transfer Learning using VGG16 pre-trained model with 2 Dense layers and Dropout.
   - **Test Accuracy:** 89.4%

6. **Final Model**

   - **Architecture:** Transfer Learning using VGG16 pre-trained model with Fine Tuning and 3 Dense layers with Dropout.
   - **Test Accuracy:** 91.1%

#### Conclusion

The project experimented with various deep learning architectures and techniques, including baseline models, regularization, transfer learning using VGG19 and VGG16, and fine-tuning. The final model achieved the highest test accuracy of 91.1%, indicating its effectiveness in classifying geospatial terrain images.







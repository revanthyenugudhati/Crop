# crop
# Introduction
In the face of global population growth and climate change, plant breeders and agronomists strive for improved crop yields and quality to ensure regional food security, regulate the market price of the rice grain, and address food-shortage problems. The rice-panicle density is one of the important agronomic components in understanding the grain yield and determining the growth period Computer-vision methods based on high-spatial-resolution images provide a potential solution to increase the throughput and the accuracy . With the development of deep learning methods, convolutional neural networks have been shown to outperform human beings in diverse fields.
The project uses low-cost remote sensors to deliver easy to understand, robust information to farmers enabling the precision application of fertilizer and other inputs. guidelines will be developed to indicate plant health and growing condition, nutrient and water deficiencies/excesses. The final product will be a mobile application and a web browser-based information dashboard that compares baseline dataset and farmer’s images and provides site-specific information and advice!
<p align="center">
  <img 
    width="600"
    height="500"
    src="https://user-images.githubusercontent.com/28043714/157062715-f76b571f-33f6-4eb0-a00b-6f50f1e3cc6d.png"
    title="System Architecture"
  >
</p>
The system architecture defines  the structure of the proposed system in which it contains the mobile application with the storage and backend ML model. The features that I want to include in this are like getting the number of leaves, the soil content which will be taken into consideration and the model will be developed. 

# Methodology

The user can access the mobile application to get the result which will be processed and stored in the application for the future use.There are different libraries in python to extract colour bands from the Image. They are like GDAL/OGR, Pyproj, Rasterio, Geopandas. The multispectral images contains 3 to 10 bands in which Near Infrared, red and green bands are helpful as they are more sensitive for the changes in the plant. Once the band is extracted we calculate the NDVI, Simple Ratio 1 and Simple Ratio 2. Calculating the Normalized Difference Vegetation Index NDVI, Simple Ratio 1 and Simple Ratio 2 which helps in getting the health of the plant. These can be calculated by using the Colour bands. Those Colour bands that are used to get the are Near-Infrared, Red and Green  colour bands from the images. The NIR plays the main important role in defining the plant health as the NIR reflects the light more and gets the health of the plant. This NIR and given and used in the formula or NDVI and Simple ratios to get the health of the plant.

<p align="center">
  <img 
    width="400"
    height="400"
    src="https://user-images.githubusercontent.com/28043714/157067705-b2cb66ed-4334-4e97-a743-96328cd746ee.png"
    title= "Flow Diagram"
  > 
</p>

The image capture is preprocesses using otsu alogrithm and masks are used to define the plant area. Once plant area is confirmed the areas are calculated and the values like color and texture are takeng from image and then a dataset is created. Once data set is created the data is set for machine learning. We have used techniques like SVM, KNN classifier. We get best results for the given data.

# Libraries & MachineLearning Models
cv2 : To work on Images
numpy & pandas : For working arrays and numerical values
mahotas : For extracting features
matplotlib: For plotting graphs
shutil : For working on folders (copying images)

### Ml models:
Suppor Vector Machine, Logistic Regression, KNN classifier

# Acknowledgement
Throughout the research I have received a great deal of support and assistance.I would like to thank Faculty of Research and Faculty of Science and Environment for funding my research. I would like to thank my supervisors, Dr. Sabah Mohammed, for his guidance through each stage of the process and Dr. Muditha Heenkenda for support for providing hardware \& data required for research.

# AI-GVI
An analysis of GVI using Google Street View tiles vs Sentinel-2 NDVI.

#### Replication Steps:
1. Run get_gee_image.ipynb[https://colab.research.google.com/drive/1E3yR3dqGDhpvyDkvF9OcpKBk_sUBJcS9?usp=sharing] in Colab to download the Google Earth Engine Sentinel-2 Image.
2. Run calculate_ndvi.ipynb locally to get the tiff file containing the ndvi.
3. Run get_gsv_image.ipynb locally to get a folder of gsv images based on the shapefile in sg_data.
4. Run calculate_gvi.ipynb[https://colab.research.google.com/drive/1RodUcEXyNxj8P409FJVBStC1b6d0WOM-?usp=sharing] in Colab to download the pretrained RNN and calculate the GVI for each tile.
5. Load the model results back into get_gsv_image.ipynb to build the final tiff file containing the calculated GVI. 

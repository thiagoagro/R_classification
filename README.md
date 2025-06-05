# 🌍 Drone Image Processing Course: Soil Removal with R 🚁

## Welcome to the Drone Image Processing! 📸
✨ This repository contains all the code and resources for learning how to process drone-captured images and remove soil using the power of R! 
🖥️🌱 Whether you're a beginner or an advanced user, this course will guide you through image preprocessing, soil segmentation, and result visualization with hands-on scripts. 🛠️📊
Get ready to dive into the world of geospatial analysis and drone imagery! 🚀 Explore the scripts, follow the course schedule, and start mastering image processing today! 🌟

## 📋 Course Workflow
Below is the step-by-step sequence of the course, guiding you through the process of soil removal in drone imagery using R:


* 📦 1 - Install Packages: Install essential R packages for image processing and analysis.
* 📚 2 - Load Libraries: Import the required R libraries for the workflow.
* 🖼️ 3 - Import Multispectral Bands: Load individual multispectral bands separately.
  * 🖼️ 3.1 - Import Orthomosaic: Directly load the orthomosaic image for analysis.
  * 🖼️ 3.2 - Visualize Image: Display the image using PlotRGB for visual inspection.
  * 📷 3.3 - Locate Treatments: Identify experimental plots within the image.
  * 📍 3.4 - Crop Area of Interest: Extract the region of interest (ROI) from the orthomosaic.
* ✂️ 4 - Calculate Vegetation Indices (Optional): Compute indices like NDVI to enhance classification.
* 🌿 5 - Create Soil and Plant Samples: Generate training samples for soil and vegetation classification.
  * 🌱 5.1 - Visualize Samples: Inspect the generated soil and plant samples.
* 👀 6 - Prepare Data for Classification: Configure samples and image for model training.
  * 🛠️ 6.1 - Classify with Random Forest (RF): Use Random Forest for classification.
  * 🧠 6.2 - Classify with Support Vector Machine (SVM): Use SVM for classification.
  * 🧠 6.3 - Classify with XGBoost (XGB): Use XGBoost for classification.
  * 📈  6.4 - Visualize and Save Classifications: Display model outputs and save classified rasters.
  * 📉 6.5 - Evaluate Model Metrics: Assess performance metrics (e.g., accuracy, Kappa) for each model.
  * 📊 6.6 - Visualize Confusion Matrix: Plot confusion matrices to evaluate classification performance.
* 🌾 7 - Remove Soil with Mask: Crop the orthomosaic using the plant mask to remove soil.
  * 💾 7.1 - Save Cropped Image: Export the soil-removed raster as a new file.
* 🚜 8 - Create Treatments with FieldImageR: Generate experimental treatments using FieldImageR.
  * 🗺️ 8.1 - Load Treatments and Create Buffer: Import plot data and create buffers for analysis.
* 🌿 9 - Calculate Indices with Pliman: Compute vegetation indices using the pliman package.
  * 💾 9.1 - Save Vegetation Indices: Export calculated indices to a file.
* 📊 10 - Extract Mean Values per Treatment: Calculate average index values for each plot.
* 📈 11 - Create Dataframe and Visualize: Convert raster data to a dataframe and plot vegetation indices.



## Vegetation index (VI) using
#### Matias et al. (2020) and colaborators developed an package call FieldImageR, the package present a lot of usefull information that were combined to the actual code. One of the interest point are the vegetation index, FieldImageR is able to calcular several VI (See below):
![image](https://github.com/user-attachments/assets/ff3c86ef-a732-4f09-8d9f-fd78b28b1b08)

* Source: https://doi.org/10.1002/ppj2.20005 (See the paper and some explanations)
* Github: https://github.com/OpenDroneMap/FIELDimageR.git

#### The second interest package that combined several VI used is the Olivoto, 2024 the Pliman package. Pliman also combined RGB and multispectral index and present a wide number of VI. These VI also can complete the present in FieldimageR package offer to the user the option of included more VI in the analysis.
![RGB_1](https://github.com/user-attachments/assets/5230bf25-07c7-49fd-ad59-e67d478679c2)
![RGB_2](https://github.com/user-attachments/assets/be7e4341-0834-465a-9cb3-a2f9d3ef6daa)
![RGB_3](https://github.com/user-attachments/assets/92e59e68-4e8f-4e0a-9b82-bfe743764321)
![RGB_4](https://github.com/user-attachments/assets/69619c48-9be5-41d6-a047-f6123f525d74)
![RGB_5](https://github.com/user-attachments/assets/e452185f-d8b6-4672-ac7d-92eef83bee54)
![RGB_6](https://github.com/user-attachments/assets/3128c9cd-b302-4d7a-8236-ad4dacdb02e3)
![RGB_7](https://github.com/user-attachments/assets/4f736344-a106-46f3-9c8c-af22172a3f92)
![RGB_8](https://github.com/user-attachments/assets/e513ec20-adb2-4134-800b-f30504907aa8)
![RGB_9](https://github.com/user-attachments/assets/679f4b39-84ad-40be-a877-d92966fba510)



* Source: https://olivoto.netlify.app/post/pliman_pt_br/
* Github: https://tiagoolivoto.github.io/pliman/
* Cran: https://doi.org/10.32614/CRAN.package.pliman

## 🚀 Getting Started

Install R and RStudio, and ensure you have Git installed to clone this repository.
Setup: Clone this repository using git clone https://github.com/usuario/curso-drone-r.git and follow the script instalacao_pacotes.R to install required packages.
Course Schedule: Check the course schedule for detailed topics and script links.

Start exploring the scripts in the repository and follow the workflow above to master drone image processing! 🌟

## Follow us in the Social Media

### Exension and Research Group in Digital Agriculture (GEPAD), Federal University of Lavras, UFLA, Agriculture Department (DAG)

![new](https://github.com/user-attachments/assets/677dca36-9e3b-45a6-a039-ab5680e82ccb)
![GEPAD](https://github.com/user-attachments/assets/e52c1135-52aa-4cb1-8dfe-0709b256720c)



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
* 🌿 4 - Create Soil and Plant Samples: Generate training samples for soil and vegetation classification.
* 🛠️ 5 - Running three ML models: RF, SVMradial and XGBtree
* 💾 6 - Save the classified map
* 📉 7 - Analyzing the models metrics and confusion matrix
* 🌾 8 - Removing the soil background
* 🚜 9 - Call the treatments, transform the coordinates and applying the buffer
* 🧠 10 - Calculate the VI following (pliman package)
* 📊 11 - Extract the mean values and save (.xlsx)
* 📈 12 - Plotting the boxplot to compare the treatments


## Pay attention
The code was write under Rstudio using the Rmarkdown and R version 4.4.3
Before starting to use the code make sure you have the Rtools ---> https://cran.r-project.org/bin/windows/Rtools/rtools43/rtools.html
You need to download the same version used for R, i.e. in my case since I'm using the R 4.4.3 I needed to download the Rtools 4.3.

## Observation
The code has extra comments about the operations and functions used. However in some cases the functions can be confuse. For example:
  * 1 if you are working on Pix4D software you gonna have the multispectral bands separate, thus you can import each one and join the bands in Rstudio.
  * 2 Creating samples is wide tool and you can create more samples than "soil" and "plants"
  * 3 Running ML models accept only three models SVM, XGB and RF or you can Run only one model
  * 4 When you call your plots or treatments, previous prepared in QGIS (for example), you need to check the coordinates system and also transform the ortosolo (soil background removed ortomosaic). Nevertheless, if you processed the images using the metashape you should know you need to transform the 16bit values for 0 - 1 normalized values for reflectance otherwise your VI showed wired values. Look at the metashape tutorial ---> https://agisoft.freshdesk.com/support/solutions/articles/31000148780-micasense-rededge-mx-processing-workflow-including-reflectance-calibration-in-agisoft-metashape-pro


## Vegetation index (VI) using
#### Matias et al. (2020) and colaborators developed a package call FieldImageR, the package present a lot of usefull information that were combined to the actual code. One of the interest point are the vegetation index, FieldImageR is able to calcular several VI (See below):
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



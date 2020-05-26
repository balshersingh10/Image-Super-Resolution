![Image-Super-Resolution]()
# Image Super Resolution Using Supervised Machine Learning Techniques
We obtained the Super Resolution Images Dataset from **http://mmlab.ie.cuhk.edu.hk/projects/SRCNN.html** and used Jupyter Notebook as the platform for the purpose of coding. Our methodology involves use of Convolutional Neural Network for Image Restoration.
## A. Feature Selection
Feature selection is finding the subset of original features by different approaches based on the information they provide, accuracy, prediction errors.
The features used in the project are Image quality metrics:
- PSNR
- MSE
- SSIM
## B. Model Selection
SRCNN model with:
* Model type -> Sequential
* Conv2D layer(activation=relu, kernel_size = (9, 9), kernel_initializer='glorot_uniform')
* Conv2D layer(activation=relu, kernel_size = (3, 3), kernel_initializer='glorot_uniform')
* Conv2D layer(activation=linear, kernel_size = (5, 5), kernel_initializer='glorot_uniform')
* Optimizer -> Adam
## C. Training the models with Data
The dataset taken is from **http://mmlab.ie.cuhk.edu.hk/projects/SRCNN.html**
## D. Taining Data and Testing Data
All original images are stored in 'source' folder and then they are degraded in quality to be stored in 'image' folder.
### Then the image quality is restored:
Image restored is stored in 'output' folder.
# Result =>
Nearly same quality is given back by algorithm which was degraded. <br />

## Files included in repository are:
- **source.ipynb(Jupyter Notebook-https://jupyter.org/)**
- **source.pdf(Just a pdf print of jupyter notebook)**
- **'source' folder (Original Images)** 
- **'image' folder (Degraded Images)** 
- **'output' folder (Restored Images)** 
- **Pre-Trained weights for SRCNN model -> '3051crop_weight_200.h5'**  <br />

# Outfit Photo To Wardrobe Matching
<p>In this project, I have created a deep-learning based system that can understand which clothing items is wear by the users and, based on that it makes the decision whether the clothing item is already present in the online wardrobe or not and if not, it will automatically get added into the wardrobe by the system.</p>
<h2>Libraries Used</h2>
<ul>
  <li>Pytorch</li>
  <li>Numpy</li>
  <li>Pandas </li>
  <li>Matplotlib</li>
  <li>Sklearn</li>
  <li>Python Imaging Library</li>
  <li>OpenCV</li>
  <li>skimage</li>
</ul>
<h2>Dataset</h2>
<p>For clothing item identification and localization, I have created a custom dataset by myself. The clothing item images have been downloaded from Kaggle's InShopeClothes dataset and it gets annotated with a bounding box with the open-source tool called YoloLabel. A total of 656 images with their respective label in the dataset, out of which 586 images with their label are in the training section and the remaining 66 are in the validation section. The dataset can be downloaded from here: https://bit.ly/3eEt90Y </p>
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/dataset.png" >

<h2>Object Detection</h2>
<p>For object detection, I have used here YoloV5 mainly for its smaller size, faster computation, and state-of-the-art accuracy. The model has to get trained over 586 images for 50 epochs. The model takes 21 minutes that is 41 seconds per epoch to complete its task. The model was able to perform object detection with the following accuracy.</p>
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/result.png" >

<h2>Object Detection Result On Validation Dataset</h2>
<h3>Input:<h3>
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/validation%20dataset.png" >
<h3>Output:<h3>
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/validation%20dataset%20object%20detection.png">
  
<h2>Image Similarity</h2>
<p>For making the system understand whether the images are similar or dissimilar, here I have used Structural Similarity Index (SSIM) for scoring the similarity between the two images. The SSIM attempts to model the perceived change in the structural information of the image, whereas MSE is estimating the perceived errors. </p>  
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/SSIM.png" width="800" height="150">
  
  
  

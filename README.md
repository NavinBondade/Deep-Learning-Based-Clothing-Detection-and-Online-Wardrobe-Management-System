# Deep Learning-Based Clothing Detection and Online Wardrobe Management System
<p> 
<img src="https://zerrin.com/wp-content/uploads/2021/10/online-wardrobe-closet-organizing-app-zerrin.png" width="1000" height="580">  
This project introduces a deep learning-based system engineered to automatically identify and catalog clothing items worn by users for seamless online wardrobe management. A custom dataset comprising 656 annotated images of various clothing categories was developed specifically for this application. The YOLOv5 model was trained on this dataset to achieve high accuracy in object detection, enabling the system to recognize and localize clothing items within images. Once identified, the system checks whether the detected items already exist in the user's online wardrobe. If an item is not found, it is automatically added, streamlining the wardrobe management process. This system offers an efficient solution for maintaining an organized and up-to-date digital wardrobe.</p>
<h2>Libraries Used</h2>
<ul>
  <li>Pytorch</li>
  <li>YoloV5</li>
  <li>Numpy</li>
  <li>Pandas </li>
  <li>Matplotlib</li>
  <li>Sklearn</li>
  <li>Python Imaging Library</li>
  <li>OpenCV</li>
  <li>skimage</li>
</ul>
<h2>Dataset</h2>
<p> For the identification and localization of clothing items, I have developed a custom dataset. The images used were sourced from Kaggle's InShop Clothes dataset, and each image has been annotated with bounding boxes using the open-source tool YoloLabel. The dataset consists of 656 images along with their corresponding labels. Of these, 586 images are allocated to the training set, while the remaining 66 images are designated for validation. The dataset is available for download at the following link: https://bit.ly/3eEt90Y </p>
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/Clothing%20Dataset.png" >

<h2>Object Detection</h2>
<p>For the object detection task, I utilized YOLOv5, chosen primarily for its compact size, rapid computation, and state-of-the-art accuracy. The model was trained on a dataset of 586 images over the course of 50 epochs. The entire training process was completed in 21 minutes, equating to an average of 41 seconds per epoch. This efficiency highlights YOLOv5's capability to balance speed and accuracy effectively. Upon completion, the model demonstrated impressive object detection performance, achieving high accuracy levels, making it well-suited for practical applications where both speed and precision are crucial.
</p>
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/result.png" >

<h2>Object Detection Result On Validation Dataset</h2>
<h3>Input:<h3>
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/Clothing%20%20Validation%20Dataset.png" >
<h3>Output:<h3>
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/Clothing%20Validation%20Dataset%20Result.png">
  
<h2>Image Similarity</h2>
<p>For making the system understand whether the images are similar or dissimilar, here I have used Structural Similarity Index (SSIM) for scoring the similarity between the two images. The SSIM attempts to model the perceived change in the structural information of the image and based on that generates a score. </p>  
<p align="center">  
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/SSIM.png" width="650" height="120">
<p>  
 
<h2>Online Wardrobe Management</h2>
<p>To efficiently manage an online wardrobe and incorporate newly detected clothing items, I developed a logical algorithm that compares each detected item against existing items in the wardrobe. This comparison is based on the Structural Similarity Index Measure (SSIM) score, which evaluates the similarity between images. If the SSIM score exceeds a predefined threshold, indicating that the new item is sufficiently distinct from the existing ones, it is added to the wardrobe. Otherwise, the item is not included, ensuring that the wardrobe remains organized and free of duplicate or similar items. This method enhances the wardrobe's functionality by maintaining a diverse and unique collection of clothing items.</p>
<h3>Current Wardrobe:</h3>  
<p align="center">  
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/Current%20Wardrobe.png">
<p>  
<h3>User Clothing Item:</h3>  
<p align="center">  
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/Users%20Clothing.png" width="450" height="450">
<p>
<h3>User Clothing Item Detected:</h3>  
<p align="center">  
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/Users%20Clothing%20Detected.png" width="450" height="450">
<p>     
<h3>Updated Wardrobe:</h3>  
<p align="center">  
<img src="https://github.com/NavinBondade/Navin_Bondade_ML_Assignment_July2021/blob/main/Images/Current%20Wardrobe1.png">
<p>   
  
<h2>Conclusion</h2>  
<p>In this project, I developed a sophisticated system that leverages YOLOv5 for the identification of clothing items, seamlessly integrating them into an online wardrobe. The system efficiently detects and recognizes clothing items using YOLOv5’s advanced object detection capabilities. It then cross-references the detected item with existing items in the wardrobe to ensure uniqueness. If the item is not already present, it is automatically added to the wardrobe, maintaining an organized and comprehensive collection. This approach not only optimizes wardrobe management but also ensures that only new and distinct items are included, enhancing the overall user experience.
</p>  
<h2>References</h2>  
https://www.kaggle.com/rvnrvn1/inshopclothes <br>
https://github.com/developer0hye/Yolo_Label <br>
https://github.com/ultralytics/yolov5 <br>
https://medium.com/srm-mic/all-about-structural-similarity-index-ssim-theory-code-in-pytorch-6551b455541e <br>
  
  

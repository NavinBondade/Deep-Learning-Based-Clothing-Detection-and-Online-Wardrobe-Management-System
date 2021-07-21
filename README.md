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
<p>For clothing item identification and localization, I have created a custom dataset by myself. The clothing item images have been downloaded from Kaggle's InShopeClothes dataset and it gets annotated with a bounding box with the open-source tool called YoloLabel. A total of 656 images with their respective label in the dataset, out of which 586 images with their label are in the training section and the remaining 66 are in the validation section. </p>


Dataset Link: https://drive.google.com/drive/folders/1t_qSYVZjEFeZXBrqLUxXSQseGOCY1YvY?usp=sharing

# MEAD-3D
* This dataset contains 3D reconstructions of the [MEAD dataset](https://wywu.github.io/projects/MEAD/MEAD.html), using the monocular 3D reconstruction algorithm in the paper **'Speech4Mesh: Speech-Assisted Monocular 3D Facial Reconstruction for Speech-Driven 3D Facial Animation' [ICCV 2023]**.

![Comparison of the reconstruction results on MEAD (left) and VoxCeleb2 (right) datasets.](https://github.com/haonanhe/MEAD-3D/blob/main/3DReconstructionCompare-names.png)
  
* The dataset can be downloaded via [BaiduNetDisk](https://pan.baidu.com/s/1rJzDlOiJXtcDctt1aFSpKA?pwd=joi4).  


* The dataset is organized as below:
    >MEAD-3D
    >>Speaker ID
    >>>video
    >>>>camera angle
    >>>>>type of emotion
    >>>>>>intensity level
    >>>>>>>video_id.npy  


* Each `.npy` file contains the following contents:

 keys  | values  | descriptions
 ---- | ----- | ------  
 'verts'  | (N, 5023, 3) | vertices reconstructed from each image 
 'beta'  | (43, 156) | 3DMM parameters (shape, expression, pose) of the [FLAME](https://flame.is.tue.mpg.de/) reconstruction 

<!--
# 'images'  | (N, 3, 224, 224) | cropped images from MEAD datasets
# 'kpt'  | (N, 68, 3) | detected key points of each image 
# 'audio'  | (S,) | corresponding audio
-->

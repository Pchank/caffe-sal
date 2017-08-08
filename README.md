IIAU (2017) Saliency Detection Models

Introduction
----------------------------------------------------------------------------------
  This file contains saliency detection models using the caffe framework. We dive into
the convolutional features in pre-trained FCN models and propose the following methods.
1) Amulet

Title: Amulet: Aggregating Multi-level Convolutional Features for Salient Object Detection
Author: Pingping Zhang, Dong Wang, Huchuan Lu, Hongyu Wang and Xiang Ruan 

2) UCF

Title: Learning Uncertain Convolutional Features for Accurate Saliency Detection
Author: Pingping Zhang, Dong Wang, Huchuan Lu, Hongyu Wang and Baocai Yin

How to use
-----------------------------------------------------------------------------------
Prerequisites: Follow the offical websites of Caffe framework and install the whole toolbox 
(necessary Matlab wrappers)

1) training

  The training code is in ./models/Amulet and ./models/UCF. For saving memory, we use the 
BN method implemented by Alex Kendall etal. The training is followed as examples in Caffe. 
The only need is changing the path of data and files.

2) testing

 The testing code is in ./matlab/Amulet_test and ./models/UCF_test. 
 
For dataset testing, 

  (1) Get prediction : test_saliency_dataset.m
  
  (2) Get PR value : PR.m
  
  (3) Plot PR curves: code_pr.m
  
  (4) Plot Bar figures: code_bar.m
  
  (5) Get MAE for each method : getmae.m
  
Note that we have provided the PR curves in ./PR_curves

Citation
-----------------------------------------------------------------------------------
Please cite the following papers if our models help your research:

@article{pingping2017amulet}

 author = {Pingping Zhang, Dong Wang, Huchuan Lu, Hongyu Wang and Xiang Ruan}
 
 journal = {arXiv preprint arXiv:1708.02001}
 
 title = {Amulet: Aggregating Multi-level Convolutional Features for Salient Object Detection}
 
}

@article{pingping2017ucf}

 author = {Pingping Zhang, Dong Wang, Huchuan Lu, Hongyu Wang and Baocai Yin}
 
 journal = {arXiv preprint arXiv:1708.02031}
 
 title = {Learning Uncertain Convolutional Features for Accurate Saliency Detection}
 
}

Question and Connection
----------------------------------------------------------------------------------
If any question, please connection

jssxzhpp@gmail.com;jssxzhpp@mail.dlut.edu.cn

---
title: Applications of Three-dimensional Freehand Portable Ultrasound
date: 2020-12-01
image:
  focal_point: 'top'
---

- ## <b>1. Introduction : </b>

    - As a non-invasive and fast imaging method, ultrasound is widely used in medical examinations.
    - 3D ultrasound (US) imaging technique has shown comparable measurement results to the radiographic method.
    - Portable ultrasound combined with deep learning technology has greatly promoted large-scale disease screening and has a wide range of applications. <br>
- ## <b>2. Pipeline : </b> {{< figure src="1.jpg" caption="Pipeline" numbered="true" >}}

    - <b>Background</b> : 2D US can just provide limited information for diagnosis of various disease and examining a large number of patients in the community is very costly and time-consuming for doctors.
    - <b>Objective</b> : Develop a set of smart devices and algorithms to realize automatic screening of people in a wide range of communities.
    - <b>Method</b> : 
        - 1. Acquire carotid artery images(shown above) from portable 3D ultrasound equipment. 
        - 2. Using deep learning to segment ROI automatically. 
        - 3. 3D reconstruction using 3D position information 
        - 4. 3D morphology analysis 
        - 5. Using deep learning to diagnosis disease automatically. The pipeline is shown above. <br>
- ## <b>3. Method : </b>
    - <b>Image acquisition</b> {{< figure src="2.jpg" caption="Freehand Portable Ultrasound" numbered="true" >}}
        - 2D images and position information are gotten from 3D portable ultrasound device.
    - <b>2D image segmentation</b> {{< figure src="3.jpg" caption="UNet for 2D image segmentation" numbered="true" >}}
        - U-shape based neural network and its variant are used for 2D US image segmentation. The architecture of network is shown above.
    - <b>3D reconstruction</b> {{< figure src="4.jpg" caption="FDP-VNN for 3D reconstruction" numbered="true" >}}
        - FDP-VNN algorithm is used for volume reconstruction after segmentation. The process of reconstruction is shown above.
    - <b>3D morphology analysis</b>
        - After getting 3D volume, morphology analysis is performed to get more useful information to diagnosis.
    - <b>Diagnosis</b>
        - Automatic diagnosis of diseases using reconstructed three-dimensional volume and three-dimensional morphological analysis. <br>
- ## <b>4. Applications : </b>
    - <b>Carotid artery ultrasound</b> {{< figure src="5.jpg" caption="Carotid artery ultrasound" numbered="true" >}}
    - <b>Gastric ultrasound</b> {{< figure src="6.jpg" caption="Gastric ultrasound" numbered="true" >}}
    - <b>Cervical Spine Ultrasound</b> {{< figure src="7.jpg" caption="Cervical Spine Ultrasound" numbered="true" >}}

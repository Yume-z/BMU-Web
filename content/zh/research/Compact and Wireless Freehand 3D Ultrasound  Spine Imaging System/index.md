---
title: Compact and Wireless Freehand 3D Ultrasound Spine Imaging System

date: 2020-12-01
image:
  focal_point: 'top'
---
- ## <b>Introduction : </b>

    - The developed 3D ultrasound spine imaging system consisted of three main components: integrated imaging equipment, fast imaging method and high-quality reconstruction algorithm. This system can realize:
        - Unconstrained multi-dimensional, multi-angle scanning
        - Intelligent and customized 3D ultrasound data acquisition
        - Fast and high-quality 3D reconstruction based on real location<br>

- ## <b>3D Ultrasound Spine Imaging Equipment</b> {{< figure src="1.jpg" caption="3D Ultrasound Spine Imaging Equipment" numbered="true" >}}

    - <b>Background</b> : Present spine imaging apparatus is bulky and inconvenient for fast and mobile scan, the scanning equipment is not transportable.<br>
    - <b>Objective</b> : Develop a new compact and wireless system to offer the real-time visualized spine images during data acquisition and the post high-quality reconstruction after acquisition.<br>
    - <b>Method</b> : The data acquisition equipment was comprised of a WIFI based 2D ultrasound scanner and a wireless portable EM tracking unit, which provided the 2D transverse images from WIFI transmission and the corresponding spatial trajectory through the 2.4G communication module, respectively. Then, the acquired data was fused to produce the 3D spine volume. 


- ##  <b>Fast-Dot Projection Method for Fast Spine Imaging</b>

    - <b>Background</b> : Present spine imaging apparatus is bulky and inconvenient for fast and mobile scan, the scanning equipment is not transportable.<br>

    - <b>Objective</b> : Develop a new compact and wireless system to offer the real-time visualized spine images during 
    - <b>Method</b> : The data acquisition equipment was comprised of a WIFI based 2D ultrasound scanner and a wireless portable EM tracking unit, which provided the 2D transverse images from WIFI transmission and the corresponding spatial trajectory through the 2.4G communication module, respectively. Then, the acquired data was fused to produce the 3D spine volume. <br>   
    {{< figure src="2.jpg" caption="Fast-Dot Projection" numbered="true" >}}
    - <b> Results</b> : Twenty clinical datasets from scoliosis patients were used for this study. The FDP-based algorithms were approximately faster by a factor of 5 as compared to the conventional algorithms, e.g., 26 sec for FDP-VNN versus 136 sec for VNN. Left (a) (b) and (c) shows the visualization results. In addition, the accelerated method was also demonstrated to provide the immediate processing while scanning (right (a) (b) and (c)).
    {{< figure src="3.jpg" caption="Results" numbered="true" >}}


- ##  <b>Neural Radiance Filed Method for High-Quality Spine Reconstruction</b>


    - <b>Background</b> : The existing reconstruction algorithm is greatly affected by the soft tissue. <br>
    - <b>Objective</b> : Apply neural radiance field (NeRF) method to improve the quality of reconstruction. <br>
    - <b>Method</b> : The procedure of spine reconstruction with NeRF was shown as below. The 2D transverse frames data and the corresponding location data were sent into the input layer for sampling. The hidden layer included  a 8-layers fully-connected multilayer perceptron . The final prediction density and weights were calculated and rendered from output layer. <br>
    - <b> Results</b> : NeRF could suppressed soft tissue interference in volume rendering result. 
    {{< figure src="4.jpg" caption="Neural Radiance Filed Method for High-Quality Spine Reconstruction" numbered="true" >}}

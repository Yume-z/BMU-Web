---
title: Learning-based frameworks for automatic spinal curvature measurement on 3D ultrasound images
date: 2020-12-02
image:
  focal_point: 'top'
---


- ## <b>1. Introduction : </b>
    - Proxy Cobb angle measured on ultrasound images can be used for diagnosing and monitoring spinal curvature. 
    - Spinous process angle (SPA) defines the posterior deformity of spine, and reveal the information of both the axial vertebral rotation and lateral curvatures.
    - The manual measurement of spine curves depends on the trained specialists, and takes great amount of time with unstable results. <br>
- ## <b>2. Objectives : </b> 
    - To automatically measure proxy Cobb angle and SPA on ultrasound images, we propose an automatic vertebral structure detection network based on convolutional neural network (CNN) and Transformer.<br>
- ## <b>3. Method : </b>
    - <b>Automatic proxy Cobb angle measurement on coronal image</b> {{< figure src="1.jpg" caption="Automatic proxy Cobb angle measurement on coronal image" numbered="true" >}}
    - <em> <b>DEtection Transformer (DETR): </b> </em> detect the lamina pairs. 
    - <em> <b>Automatic SPA measurement on 3D ultrasound images: </b> </em> 
    {{< figure src="2.jpg" caption="Stacked hourglass Network" numbered="true" >}}
        - <em> <b>Input </b> </em>: a transverse ultrasound image, whose (spinous process) SP and lamina are labeled as five landmarks (red dots).<br>
        - <em> <b>Detector </b> </em>: predict coordinates of SP and lamina.<br>
        - <em> <b>Classifier </b> </em>: give the confidence of detections by categorizing image patches, which are generated based on coordinates.<br>
        - <em> <b>Outputs </b> </em>: 
        {{< math >}}
        $$
        [𝐿𝐴_𝑥^𝑖,𝐿𝐴_𝑥^𝑖 ],[𝑆𝑃_𝑥,𝑆𝑃_𝑦 ],𝑃_{𝑠𝑝},𝑃_{𝐿𝐴}
        $$
        {{< /math >}}
        {{< figure src="3.jpg" caption="Pipeline" numbered="true" >}}
        - <em> <b>Without process (green) </b> </em>: SP is invisible on coronal image (a).<br>
        - <em> <b>Process entire US scan (orange)</b> </em>: each transvers image in US scan is input into detector and classifier, and will be processed as image (b) and replace original image.<br>
        - <em> <b>Measurement (blue) </b> </em>: entire US scan is reconstructed as coronal image (c), in which only SP and lamina are visible. SPA is measured automatically based on detected SP.<br>

       

- ## <b>4. Results : </b> {{< figure src="4.jpg" caption="Illustration of automatic measurement" numbered="true" >}}
    - <b>Illustration of automatic measurement:</b> 
      - (a)-(c) proxy Cobb angle, (d)-(g) SPA. 
      - The detected spine curves match the spinal curvature. 
      - As shown in the white box, the SP curves reveal apparent vertebral rotation and are deviated to the same direction on e&g.
    {{< figure src="5.jpg" numbered="true" >}}
    - <b>Comparison between US and radiographic measurement: </b> 
      - Correlation: (a) US proxy Cobb vs X-ray Cobb, (b) manual US SPA vs X-ray SPA, and (c) auto US SPA vs X-ray SPA.
      - The mean absolute difference (MAD) between SPAs from US and radiographic method was 3.5±2.5°.


- ## <b>5. Conclusion : </b>
    - The proxy Cobb angle and SPA can be measured automatically on the 3D US images, and the error was less than clinical acceptance error (5°). 
    - The automatic method can be regarded as a reliable and promising tool for the diagnosis, monitoring and screening of spine deformities.

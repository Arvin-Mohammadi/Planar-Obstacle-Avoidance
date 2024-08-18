# Planar Obstacle - Avoidance (Application in Delta Robot)

</br>
<p align="center">
	<strong><a href="https://github.com/Arvin-Mohammadi/Planar-Obstacle-Avoidance/tree/main/Research">FULL RESEARCH OUTLINE</a></strong>
</p>
</br>


<img align="right" src="https://github.com/Arvin-Mohammadi/Delta-Robot-Trajectory-Planning-V3/assets/69509720/5d0b34e0-8cbd-4d3d-9884-382a565008ef" width=20%>


Overview: 
- [introduction](#section-introduction)
- [object detection](#section-object-detection)
- [grid problem](#section-grid-problem)
- [trajectory generation](#section-trajectory-generation)
- [references](#section-references)
</br>


























<a name="section-introduction"></a>
# Introduction

Here's the overall idea for a 2D-viewed obstacle avoidance algorithm. 

|                     <img src="https://github.com/user-attachments/assets/ca08bfa9-dfaf-461e-9ff0-a72e09ef630a" style="width: 85%;">                     |                     <img src="https://github.com/user-attachments/assets/0025891b-acee-48d1-9c8e-8e42324ce902" style="width: 85%;">                    |
|:--------------------------------------------:|:-------------------------------------------:|
|     Workspace (Initial and Final Points)     | Object Detection and Blocking Out Obstacles |
|                     <img src="https://github.com/user-attachments/assets/ccd4fafa-be7d-4123-80c2-5ce6156781d9" style="width: 85%;">                     |       <img src="https://github.com/user-attachments/assets/92029b69-6731-490f-93f4-5650755c2c0a" style="width: 85%;">                                  |
| Grid Modeling and Extracting Key Path Points |            Trajectory Generation            |





















<a name="section-object-detection"></a>
# Object Detection

For using the Yolo-V5 we're going to take the following steps ([Reference #1](#reference-yolov5)):
- Python Virtual Environment Setup
- Installing Pytorch and Cuda
- Use the Default Yolo-V5 Model


</br>
<p align="center">
	<strong><ins><a href="https://github.com/Arvin-Mohammadi/Planar-Obstacle-Avoidance/tree/main/Research/Python%20Virtual%20Environment">Step 1: Python Virtual Environment Setup</a></ins></strong>
</p>
</br>

it is advised to setup a virtual environment before using Pytorch and Cuda.

</br>
<p align="center">
	<strong><ins>Step 2: Installing Pytorch and Cuda</ins></strong>
</p>
</br>

First go to the [Pytorch Local Installation](https://pytorch.org/get-started/locally/) address. In the following section choose the appropriate installation version for your computer. Copy the output command and run it in your Virtual Env.

![image](https://github.com/user-attachments/assets/cd2244f5-8eca-4c03-b970-f91494ca6c5c)

For installing the GPU-activated version you'll need cuda which you can find in the [CUDA Download Page](https://developer.nvidia.com/cuda-11-8-0-download-archive?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exe_local)


</br>
<p align="center">
	<strong><ins>Step 3: Use the Default Yolo-V5 Model</ins></strong>
</p>
</br>

The following [jupyter notebook](https://github.com/Arvin-Mohammadi/Planar-Obstacle-Avoidance/blob/main/Code/Obstacle%20Avdoidance.ipynb) contains the code necessary code for using Yolo-V5 for a given image under the section "Object Detection". 

</br>
<div align="center">
 	<img src="https://github.com/user-attachments/assets/53326845-e5d0-46df-be72-8a6999ef46e5" width=100%>
</div>
</br>




























<a name="section-grid-problem"></a>
# Grid Problem and Search Algorithms

A search algorithm that is typically used for finding the path in graph, or in this case a grid-world, is called Breath-First Search (BFS) Algorithm. 

</br>
<div align="center">
 	<img src="https://github.com/user-attachments/assets/0194d572-a7a0-4bb5-b729-2419bba5eaa8" width=50%>
	</br>
	BFS Algorithm <a href="https://en.wikipedia.org/wiki/Breadth-first_search">img reference</a>
</div>
</br>


The following [jupyter notebook](https://github.com/Arvin-Mohammadi/Planar-Obstacle-Avoidance/blob/main/Code/Obstacle%20Avdoidance.ipynb) contains the code necessary code for using BFS Algorithm in a grid-world under the section "Grid Search". 


</br>
<div align="center">
 	<img src="https://github.com/user-attachments/assets/cf402a1e-15c6-4d04-b080-65242266548e" width=50%>
</div>
</br>


























<a name="section-trajectory-generation"></a>
# Trajectory Generation


























<a name="section-references"></a>
# References

<a name="reference-yolov5"></a>
[1] [YOLO-V5 Ultralytics](https://github.com/ultralytics/yolov5)
























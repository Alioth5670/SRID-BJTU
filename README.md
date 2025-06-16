# 🚄 SRID-BJRU: A Simulation Framework and Dataset for Railway Intrusion Detection

## Download
[Google Drive](https://drive.google.com/drive/folders/1HyAO2aniWTGOlI99I55eidfwwHQhABTD?usp=sharing)  
[Baidu Drive](https://pan.baidu.com/s/16I0QVheeJeZLkoA2t8RRHw) Password: 7ua3


## Dataset Description

### Overview

**SRID-BJTU** is a synthetic railway intrusion detection dataset designed for safety monitoring, featuring diverse railway scenes such as tunnels, bridges, and intersections under various environmental conditions.

<p align="center">
    <img src="figures/scene_sample.png" alt="Figure 1: Schematic illustrations of selected primary railway scenes" width="70%" />
</p>

We simulated various illumination settings, including daytime, dawn/dusk, and nighttime, to evaluate the performance of detection algorithms under different lighting conditions.

<p align="center">
    <img src="figures/time_of_day.png" alt="Figure 2: Visual changes under different time-of-day conditions" width="50%" />
</p>



### Data Collection and Annotation

We collected **7,142** annotated images. The table below provides detailed information regarding the number of images and object bounding boxes across different scenarios.

<p align="center">
    <img src="figures/detailed_information.jpg" alt="Table: SRID-BJTU Detailed Information" width="80%" />
</p>

A total of **11,898 bounding boxes** were automatically generated, following the MS COCO metrics.

<p align="center">
    <img src="figures/coco_form_size_distribution.jpg" alt="Table: Size distribution based on MS COCO metrics" width="60%" />
</p>

The following figure shows the distribution of all annotation boxes in the dataset:

<p align="center">
    <img src="figures/distribution.png" alt="Table: distribution of annotations" width="90%" />
</p>

## Experiment Result

### Object detection experimental results of training and validation on simulated dataset.

<p align="center">
    <img src="figures/tab_sim_det.jpg" alt="Table: Object detection results (simulated)" width="70%" />
</p>
<p align="center">
    <img src="figures/sim_det.png" alt="Figure: Simulated detection results" width="70%" />
</p>



### Object detection experimental results of training on only real dataset and using simulated data as data augmentation, validation on real dataset.

<p align="center">
    <img src="figures/tab_real_det.jpg" alt="Table: Real dataset + simulated augmentation" width="70%" />
</p>
<p align="center">
    <img src="figures/real_det.png" alt="Figure: Real detection results with simulation augmentation" width="70%" />
</p>



### Semantic segmentation experimental results of training and validation on simulated dataset.

<p align="center">
    <img src="figures/tab_sim_seg.jpg" alt="Table: Semantic segmentation results (simulated)" width="70%" />
</p>
<p align="center">
    <img src="figures/sim_seg.png" alt="Figure: Simulated segmentation results" width="70%" />
</p>



### Semantic segmentation experimental results of training on only real dataset and using simulated data as data augmentation, validation on real dataset.

<p align="center">
    <img src="figures/tab_rs_seg.jpg" alt="Table: Real dataset + simulated augmentation (segmentation)" width="70%" />
</p>
<p align="center">
    <img src="figures/rs_seg.png" alt="Figure: Real segmentation results with simulation augmentation" width="70%" />
</p>


## 📚 References

- [YOLOv5](https://github.com/ultralytics/yolov5) – Ultralytics
- [YOLOv8](https://github.com/ultralytics/ultralytics) – Ultralytics
- [Faster R-CNN](https://arxiv.org/abs/1506.01497) – Girshick et al.
- [RT-DETR](https://arxiv.org/abs/2304.080692) – Carion et al.
- [DeepLabV3+](https://arxiv.org/abs/1802.02611) – Chen et al.
- [SegFormer](https://arxiv.org/abs/2105.15203) – Xie et al.
- [Mask2Former](https://arxiv.org/abs/2112.01527) – Cheng et al.
- [RailSem19 Dataset](https://ieeexplore.ieee.org/document/90256469) – Zendel et al.

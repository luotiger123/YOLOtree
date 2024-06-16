# YOLOTree-Individual tree Spatial Positioning and Crown Volume Calculation Using UAV-RGB Imagery and LiDAR Data

## Study area
![image](datasets/area.png)
![image](datasets/big.png)

## Contrast Experiment
| Model | Dataset | precision/% | recall/% | mAP50/% | mAP50-95/% |
| :----: | :----: | :----: | :----: | :----: | :----: |
| YOLOv3 | TreeLD | 88.77 | 92.82 | 93.23 | 46.60 |
| YOLOv5 | TreeLD | 90.44 | 91.78 | 95.58 | 51.95 |
| Yolov7 | TreeLD | 89.84 | 90.8 | 94.73 | 49.91 |
| YOLOv8 | TreeLD | 89.71 | 91.22 | 95.33 | 52.93 |
| YOLOv9 | TreeLD | 90.13 | 90.32 | 95.04 | 53.96 |
| Faster-RCNN | TreeLD | 83.94 | 94.96 | 83.94 | / |
| YOLOTree(ours) | TreeLD | 90.52 | 91.14 | 95.53 | 52.84 |

| Model | E_neck | E_detect | E_backbone | BiFPN | precision/% | recall/% | mAP50/% | mAP50-95/% | parameters/Mb | GFLOPs
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| YOLOv8n |  |  |  |  | 89.8 | 91.4 | 95.3 | 52.9 | 3.0 | 8.1 |
| YOLOv8s |  |  |  |  | 90.5 | 91.0 | 95.6 | 53.2 | 11.1 | 28.4 |
| YOLOv8m |  |  |  |  | 89.9 | 91.4 | 95.4 | 53.2 | 25.8 | 78.7 |
| YOLOv8n | ✓ |  |  |  | 89.7 | 91.2 | 95.3 | 52.9 | 3.0 | 8.3 |
| YOLOv8s | ✓ |  |  |  | 89.6 | 90.9 | 95.1 | 52.8 | 11.2 | 29.3 |
| YOLOv8n |  | ✓ |  |  | 89.5 | 91.0 | 95.0 | 52.5 | 3.0 | 8.2 |
| YOLOv8n |  |  | ✓ |  | 90.5 | 90.5 | 95.3 | 52.7 | 3.0 | 8.4 |
| YOLOTree |  |  | ✓ | ✓ | 90.5 | 91.1 | 95.5 | 52.8 | 3.0 | 8.4 |

## Test Demo
![image](datasets/test.png)
![image](datasets/test_pre.png)
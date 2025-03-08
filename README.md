# Nuclei Segmentation using Detectron2 and YOLOv8

## Dataset
The dataset used for this project can be downloaded from:
**[NuInsSeg Dataset](https://www.kaggle.com/datasets/ipateam/nuinsseg?resource=download)**

For a detailed dataset description, refer to the official paper:
**[NuInsSeg: Dataset Description](https://arxiv.org/abs/2308.01760)**

### Summary of the Dataset
The **NuInsSeg** dataset contains more than **30k manually segmented nuclei** from **31 human and mouse organs** and **665 image patches** extracted from H&E-stained whole slide images. Additionally, ambiguous area masks are provided to indicate regions where manual semantic/instance segmentation was impossible.

---
## Approach
I explored two different methods for **Nuclei Segmentation and Analysis** using **Detectron2 (Mask R-CNN)** and **YOLOv8**.

### Procedure:
1. Downloaded the dataset from Kaggle.
2. Cleaned the data and converted masks to **COCO JSON** and **YOLOv8 annotation format**.
3. Visualized the annotations.
4. Trained **Detectron2** using **Mask R-CNN** for object detection.
5. Trained **YOLOv8** for segmentation.
6. Conducted a **quantitative analysis** to compare both methods.

---

## Comparison of Results

### Detectron2 (Mask R-CNN)
![Detectron2 Output](https://github.com/kunaltilaganji/Nuclei-Segmentation-Detectron2-and-YOLOv8/blob/main/images/Screenshot.png)

### YOLOv8
![YOLOv8 Output](https://github.com/kunaltilaganji/Nuclei-Segmentation-Detectron2-and-YOLOv8/blob/main/images/images.jpg)

---
## Conclusion
Upon analysis, I observed that **YOLOv8 tends to over-segment the nuclei**, whereas **Detectron2 provides more accurate segmentation** results. Further refinements can be made to improve performance, especially for challenging cases.

---
## Dependencies & Installation
To run this project, install the required dependencies:
```bash
pip install -r requirements.txt
```


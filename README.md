----------------------------------------------------------
Task 7.1 - Brain Tumor Segmentation using YOLOv11 + SAM2
---------------------------------------------------------
This repository contains my project for Task 7.1 of the ARCH Technologies Machine Learning Internship (Intermediate Category). The goal of this project is to perform brain tumor segmentation using a combination of YOLOv11 for object detection and SAM2 (Segment Anything Model v2) for instance segmentation.

-------------------------------------------
📘 Project Overview
-------------------------------------------
This project combines two advanced models:

* YOLOv11: Used for detecting bounding boxes around brain tumors in images.
* SAM2 (Segment Anything Model): Used for segmenting tumor regions inside the detected boxes.

The task uses brain tumor images from a custom dataset and includes model training, testing, and inference.


-------------------------------------------
* 🧪 Inference Pipeline
-------------------------------------------
1. Load YOLOv11 model (with trained weights)
2. Detect tumors in test image using YOLO
3. Pass detected bounding boxes to SAM2
4. Segment tumor regions inside each box
5. Save final segmented output


-------------------------------------------
* 📂 Repository Contents
-------------------------------------------
* File/Folder Description 

| task_7_1_segmentation.ipynb` ---- Full Jupyter notebook with training + inference code |
| requirements.txt`   ------------- List of required libraries (ultralytics, torch, etc.) |
| test_images/`  ------------------ Sample brain tumor test images |
| weights/` ----------------------- Trained YOLOv11 model (`best.pt`) |
| runs/` or `results/` ------------ Output images from detection and segmentation |
| README.md` ---------------------- Project documentation 


-------------------------------------------
*---Setup Instructions---*
-------------------------------------------
```bash
pip install -r requirements.txt
```

Then open the notebook and run each cell step-by-step.

Make sure your directory structure includes:
* test_images/meningioma_3.jpg` (or any test image)
* weights/best.pt` from YOLO training
* sam2_b.pt` for SAM2 model


-------------------------------------------
💡 Learnings
-------------------------------------------
* Hands-on training and testing of YOLOv11 on medical images
* Understanding instance segmentation using SAM2
* Model inference pipeline using combined object detection + segmentation
* Real-world use case: brain tumor localization


-------------------------------------------
📚 References
-------------------------------------------
* Video Tutorial: [YOLOv11 + SAM2 Custom Instance Segmentation by Code with Arohi](https://youtu.be/Us3oB6JwwBQ?si=Hzqsyik1580t7ZfT)
* Dataset: [Roboflow - Tumor Detection YOLOv11](https://universe.roboflow.com/brain-tumor-detection-wsera/tumor-detection-ko5jp/dataset/8)
* [Ultralytics YOLOv8 Documentation](https://docs.ultralytics.com/)
* [Meta AI SAM2 GitHub](https://github.com/facebookresearch/segment-anything)

-------------------------------------------
*---Author---*
-------------------------------------------
Muhammad Owais Arshad 
ML Intern – ARCH Technologies  
BSAI Student at PAF-IAST, Haripur  

**YOLOv8 for Real-Time Object Detection in Autonomous Systems**

### Overview
This Project investigates real-time object detection using the YOLOv8 model in autonomous driving systems. Its primary objective is to improve the accuracy, efficiency, and fairness of object detection across varying environments. The project integrates advanced machine learning techniques, including data augmentation and bias mitigation, to enhance the YOLOv8 model’s performance. Additionally, object detection from video streams in real-world scenarios is explored, contributing to the development of safer and more equitable autonomous systems.

### Key Features
- **Object Detection**: Leveraged the YOLOv8 architecture to detect and classify objects in real time.
- **Data Augmentation**: Employed strategies such as Mosaic and CutMix, along with other augmentation techniques to enhance model generalization.
- **Bias Mitigation**: Incorporated fairness-aware algorithms to reduce detection bias across diverse settings.
- **Real-Time Performance**: Assessed the model's ability to function in real time, emphasizing latency and frame rate.

### Methodology

#### Data Collection & Pre-processing:
- Utilized the KITTI Object Detection dataset and a custom dataset created via Roboflow.
- Pre-processing steps included image resizing, normalization, and advanced data augmentation.

#### Model Design & Training:
- The YOLOv8 architecture was trained using transfer learning, based on pre-trained weights from the COCO dataset.
- Hyperparameters were optimized, using a batch size of 34, image resolution of 640x640, and techniques like horizontal flipping and contrast adjustment.

#### Evaluation:
- Performance metrics such as Mean Average Precision (mAP), Precision, Recall, and F1-Score were used for evaluation.
- Real-time performance was tested on live video data, focusing on frame rate (FPS) and latency.

#### Bias & Fairness:
- Bias mitigation strategies were employed to ensure equitable detection across various demographic groups and object types, using metrics such as Demographic Parity and Equal Opportunity.

### Experimental Setup
- **Hardware**: Training was conducted on Google Colab Pro, utilizing an NVIDIA Tesla T4 GPU for optimal processing.
- **Software**: The project was developed using Python, PyTorch, and the Ultralytics YOLOv8 framework.

### Results
- **Mean Average Precision (mAP)**: The YOLOv8 model demonstrated high accuracy, particularly for large objects, with some challenges in detecting smaller objects.
- **Real-Time Performance**: During real-time video inference, the model sustained an FPS of 25 with an average latency of 32.2 milliseconds per frame.
- **Bias Mitigation**: The fairness-aware algorithms improved detection of underrepresented classes, such as pedestrians and cyclists.

### Future Work
- **Improving Small Object Detection**: Enhancing the model’s ability to detect small objects through higher-resolution datasets.
- **Edge Device Optimization**: Exploring pruning and quantization for deployment on edge devices.
- **Regulatory Compliance**: Ensuring that the model adheres to legal standards for safety-critical applications.

### Conclusion
This project demonstrates the effectiveness of the YOLOv8 model for real-time object detection in autonomous systems, achieving notable improvements in performance and fairness. The results offer valuable insights for deploying AI models in real-world applications.

### Project Repository
The complete source code and dataset for this project can be accessed [here].


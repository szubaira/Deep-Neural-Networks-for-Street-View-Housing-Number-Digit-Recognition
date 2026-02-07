## **Street View House Numbers (SVHN) Classification via Convolutional Neural Networks (CNN)**

### **Project Overview**

This project focused on developing a robust deep learning solution to recognize digits in real-world imagery using the Street View House Numbers (SVHN) dataset. By implementing a **Convolutional Neural Network (CNN)**, I addressed the challenge of classifying digits (0–9) captured in natural scenes, which include significant noise and environmental variability. The final model achieved a **78% test accuracy** and an **80% F1-score**, proving that deep learning architectures can effectively navigate the complexities of real-world optical character recognition.

### **Business Understanding**

The primary stakeholders for this project include logistics companies, postal services, and municipal mapping departments (e.g., Google Street View). The business problem centers on the inefficiency and high cost of manual data entry from physical environments. Unlike standardized handwritten datasets, real-world images present challenges such as varied lighting, motion blur, and background clutter.

Research indicates that automating address extraction can significantly reduce the "last-mile" delivery error rate and accelerate document digitization workflows. Designing a system that reliably extracts numeric data under realistic conditions allows businesses to automate mail sorting and improve the accuracy of intelligent transportation systems.

### **Data Understanding**

The analysis utilized the **SVHN dataset**, which contains cropped  pixel images of digits 0–9.

* **Data Characteristics:** The dataset is derived from Google Street View imagery, featuring single digits that vary in scale, orientation, and color.
* **Timeframe/Scope:** The dataset is a benchmark collection used for evaluating supervised learning models in computer vision.
* **Limitations:** A key limitation is the presence of "distractor" digits on the sides of the primary digit, which can sometimes interfere with the spatial feature extraction of the target number.
* **EDA:** Initial exploration confirmed a varied label distribution and a wide range of pixel intensities, necessitating normalization to ensure stable model convergence.
<img width="792" height="119" alt="Screen Shot 2026-01-23 at 01 06 17" src="https://github.com/user-attachments/assets/431ca346-c666-47e2-8b55-a3fcf8d3920d" />

### **Modeling and Evaluation**

A **Convolutional Neural Network (CNN)** was constructed to capture the spatial hierarchies of the image data. The architecture integrated convolutional layers for feature detection, pooling layers for dimensionality reduction, and fully connected layers for the final classification.

* **Optimization:** Performance was fine-tuned by adjusting hyperparameters, including learning rate, batch size, and network depth.
* **Evaluation Metrics:** * **Validation Accuracy:** 76%
* **Test Accuracy:** 78%
* **F1-Score:** 80% (Achieved after hyperparameter optimization)
* **Results:** The model showed strong generalization abilities, maintaining consistent performance across diverse image conditions compared to shallower neural network architectures.
<img width="791" height="772" alt="Screen Shot 2026-01-23 at 01 05 38" src="https://github.com/user-attachments/assets/7e612f7f-e2da-4936-96d8-9e1b2c77a76f" />
<img width="785" height="536" alt="Screen Shot 2026-01-23 at 01 06 47" src="https://github.com/user-attachments/assets/b5de8351-dc95-4617-933b-38b0bb0cabc4" />

### **Conclusion**

This project demonstrates that CNNs are highly effective for extracting information from complex, noisy visual environments. To solve the business problem of automated data entry, I recommend deploying this model as a pre-processing engine for automated logistics and mapping services.

**Future Steps:**

* **Data Augmentation:** Implement random rotations, scaling, and color jitters to improve the model's robustness against extreme lighting and orientation variations.
* **Multi-Digit Recognition:** Expand the architecture to utilize a Sliding Window or YOLO (You Only Look Once) framework to detect and read sequences of digits (e.g., full house numbers) simultaneously.

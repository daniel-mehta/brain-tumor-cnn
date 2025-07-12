# Brain Tumor Classification using CNNs and Grad-CAM 🧠
> Deep learning for brain tumor diagnosis from MRI with explainable AI.


An end-to-end deep learning pipeline for classifying brain tumors from MRI scans using Convolutional Neural Networks (CNNs), enhanced with Grad-CAM visualizations and CLAHE preprocessing. Achieves 94% accuracy across four classes: **glioma**, **meningioma**, **pituitary**, and **no tumor**.

> This project was developed as part of a course in July 2025.

---

## 🧩 Features

- ✅ **High Accuracy (94%)** multi-class tumor classification
- 🎯 **Grad-CAM** heatmaps for model interpretability and clinical transparency
- ⚙️ **CNN with regularization** to prevent overfitting
- 🧪 Evaluation using precision, recall, F1-score, and confusion matrix
- 🖼️ **CLAHE preprocessing** for enhanced MRI contrast

---

## 🧠 Dataset

Sourced from Kaggle:  
**[Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)**  
- 5,712 training images  
- 1,311 testing images  
- Categories:
  - Glioma
  - Meningioma
  - Pituitary
  - No Tumor

---

## 📊 Model Architecture

CNN built using TensorFlow/Keras:
- 3 × Conv2D → MaxPooling2D → Dropout blocks
- Flatten → Dense → Dropout → Softmax
- Loss: `sparse_categorical_crossentropy`
- Optimizer: `adam`
- Metrics: `accuracy`

Final validation accuracy: **93.6%**  
Final test accuracy: **94%**

---

## 🔬 Visual Results

| Metric         | Score (Macro Avg) |
|----------------|-------------------|
| Accuracy       | 94%               |
| Precision      | 0.94              |
| Recall         | 0.93              |
| F1-Score       | 0.93              |

Grad-CAM heatmaps were applied to visualize important regions influencing predictions. See `sample_outputs/` for visual examples.

---

## 📁 Folder Structure

```bash
brain-tumor-cnn/
├── notebook/
│   └── Midterm_5502_brain_tumor_image.ipynb      # Main pipeline notebook
│
├── reports/
│   ├── 5502_Midterm_Report_Group_1.pdf           # Final report
│   ├── 5502_Midterm_Presentation_Group_1.pdf     # Final presentation (PDF)
│   └── 5502_Midterm_Presentation_Group_1.pptx    # (optional) raw slides
│
├── sample_outputs/
│   └── gradcam_example_1.png                     # Grad-CAM overlays here
│
├── README.md
```

---

## 🔗 Related Technologies

- TensorFlow / Keras  
- OpenCV  
- NumPy / Matplotlib / Seaborn  
- Grad-CAM (Selvaraju et al., ICCV 2017)



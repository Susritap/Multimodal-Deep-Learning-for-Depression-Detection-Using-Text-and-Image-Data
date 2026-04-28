# 🧠 Multimodal Depression Detection System  
## 🤖 Deep Learning using Text and Image Data

This project focuses on detecting depression using a **multimodal deep learning approach** that combines **text and image data**.  
It leverages transformer-based NLP models and CNNs to capture emotional patterns and improve prediction accuracy.

---

## 🚀 Overview

Depression is a serious mental health issue, and early detection is important for timely support.  
Most existing systems use either text or images, but this project combines both to better understand emotional signals.

This system:
- Uses **text + image data together**
- Applies **advanced deep learning models**
- Compares multiple fusion techniques
- Identifies the best model for accurate depression detection  

---

## 📁 Dataset

### 📝 Text Data
- Source: Reddit Depression Dataset  
- Total Records: 7,650  
- Classes:  
  - 0 → Non-Depression  
  - 1 → Depression  

### 🖼️ Image Data
- Source: Roboflow (Facial Expression Dataset)  
- Total Images: 562  

---

## 🔍 Project Workflow

1. Data Collection  
2. Text Preprocessing (cleaning, tokenization, padding)  
3. Image Preprocessing (resizing, normalization, augmentation)  
4. Feature Extraction  
5. Multimodal Fusion  
6. Model Training  
7. Model Evaluation  

---

## 🧠 Models Used

### 🔤 Text Models
- BERT + BiGRU  
- RoBERTa + BiGRU  
- DistilBERT + BiGRU ⭐ (Best)

### 🖼️ Image Model
- ResNet18 (Pretrained CNN)

---

## 🔗 Fusion Techniques

- Add  
- Concatenation  
- Attention  
- Concat + Attention ⭐ (Best Fusion)  
- Bilinear  
- Cross Residual Fusion  

---

## 📈 Model Performance

### 🔤 Text Models
| Model                  | F1 Score |
|-----------------------|---------|
| DistilBERT + BiGRU    | **98.78%** |
| BERT + BiGRU          | 98.52% |
| RoBERTa + BiGRU       | 98.43% |

### 🖼️ Image Model
- Accuracy: ~87%

### 🔗 Multimodal Model
| Fusion Method        | F1 Score |
|---------------------|---------|
| Concat + Attention  | **95.65%** |
| Others              | 82% – 87% |

---

## 📊 Key Findings

- Text models perform the best (~98.5% accuracy)  
- Image-only model has moderate performance (~87%)  
- Multimodal fusion improves over image-only models  
- Best fusion method: **Concat + Attention**  
- Best overall model: **DistilBERT + BiGRU**

---

## 📉 Evaluation Metrics

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- ROC-AUC  
- Confusion Matrix  

---

## 💡 Conclusion

- Text data is the strongest indicator of depression  
- Multimodal learning improves understanding but depends on fusion quality  
- Deep learning models can effectively detect depression from social media data  
- The system is accurate, reliable, and scalable  

---

## 🌐 Future Improvements

- Use larger and more diverse datasets  
- Improve fusion techniques further  
- Add audio modality (speech analysis)  
- Deploy as a real-time mental health monitoring system  

---

## 🛠️ Technologies Used

- Python  
- PyTorch / TensorFlow  
- Transformers (BERT, RoBERTa, DistilBERT)  
- CNN (ResNet18)  
- NumPy, Pandas  
- Matplotlib, Seaborn  

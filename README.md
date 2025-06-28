# Sign-Language-to-Text-Conversion-Model

A real-time deep learning system that translates American Sign Language (ASL) fingerspelling into English text using computer vision and convolutional neural networks (CNNs).

## 📌 Overview

This project bridges the communication gap between the Deaf & Mute (D&M) community and non-sign language users. By leveraging a vision-based approach, the system detects ASL hand gestures and converts them into readable English text, enhancing accessibility and inclusion.

## 🚀 Features

- Real-time ASL alphabet recognition using CNNs.
- Achieved 98% accuracy across 26 English alphabet gestures.
- Auto-correction of predicted words using Hunspell dictionary.
- Works seamlessly with standard webcams—no special hardware needed.
- Two-stage gesture classification to handle similar hand signs.

## 🛠️ Tech Stack

- **Languages**: Python  
- **Libraries & Frameworks**: TensorFlow, Keras, OpenCV, NumPy, Hunspell  
- **Tools**: Visual Studio Code, Jupyter Notebook

## 🧠 Model Architecture

- **CNN Layers** with convolution, pooling, dropout, and fully connected layers.
- **Two-tier classification** to enhance accuracy for ambiguous signs (e.g., D vs. R vs. U).
- **Input Shape**: 128x128 grayscale images.
- **Optimizer**: Adam  
- **Activation**: ReLU  
- **Final Output**: Softmax (27 classes including a blank gesture)

## 📊 Accuracy

| Layer Used       | Accuracy |
|------------------|----------|
| Base CNN Model   | 95.8%    |
| With Double Layer Classifier | **98.0%** |

## 📷 Dataset

- Custom dataset created using OpenCV.
- 800+ images per gesture for training and 200+ for testing.
- Preprocessing includes Gaussian Blur, thresholding, and resizing.

## ✍️ Sentence Formation

- Characters are recognized and concatenated after being detected consistently.
- Blank gesture used as a space indicator.
- Hunspell-based autocorrect offers suggestions for misspelled words.

## 🧩 Challenges Faced

- Lack of a raw image dataset for ASL gestures.
- Similarity in gesture shapes caused classification confusion.
- Variability in lighting and background handled through preprocessing.

## 🔭 Future Scope

- Support for dynamic gestures and sentence-level context.
- Multi-language support (e.g., Indian Sign Language).
- Deployment as a mobile or web app.
- Enhanced NLP integration for context-aware translation.

## 📄 Research Paper

A detailed project report and paper outlining methodology and results is available in the repository.

## 🙌 Acknowledgements

Special thanks to the guide and team members who contributed to this impactful project and made it a successful solution for accessibility.

---

**Contributions are welcome!** Feel free to fork the repo, suggest improvements, or raise issues.


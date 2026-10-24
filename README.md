# 👁️ Eye Disease Detection

### 🩺 AI-Powered Eye Disease Classification Using Deep Learning

An image classification project that uses **Transfer Learning with a fine-tuned ResNet34 model** to classify eye images into five categories. Built with Fastai and PyTorch, the project includes a dedicated image augmentation pipeline and a Flask web application.

<p align="center">
  <a href="https://web-production-1a232.up.railway.app/">
    <img src="https://img.shields.io/badge/🚀_Live_Demo-Try_It_Now-00C853?style=for-the-badge" alt="Live Demo"/>
  </a>
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/PyTorch-Deep_Learning-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/>
  <img src="https://img.shields.io/badge/Fastai-Transfer_Learning-00A98F?style=for-the-badge" alt="Fastai"/>
  <img src="https://img.shields.io/badge/Flask-Web_App-000000?style=for-the-badge&logo=flask&logoColor=white" alt="Flask"/>
</p>

---

## 🌐 Live Demo

**Try the deployed application:** [Eye Disease Detection — Open Web App](https://web-production-1a232.up.railway.app/)

Upload an eye image to test the application's classification workflow.

> **Disclaimer:** This project is intended for educational and research purposes only. Its predictions are not a medical diagnosis and should not replace professional ophthalmological evaluation.

---

## ✨ Key Features

- 🧠 **Transfer Learning:** Fine-tuned ResNet34 architecture for image classification.
- 👁️ **Five-Class Classification:** Predicts one of five eye image categories.
- 🖼️ **Image Augmentation:** Generates additional training images using horizontal flips and 180-degree rotations.
- 🌐 **Web Interface:** Flask application for interacting with the trained model.
- 📓 **Jupyter Notebooks:** Separate notebooks for augmentation and model training.
- 🔬 **Deep Learning Workflow:** Dataset preparation, augmentation, training, and model export.

---

## 🔍 Supported Categories

| Category | Description |
|---|---|
| 👁️ Glaucoma | Eye images associated with glaucoma |
| 🔎 Cataracts | Eye images associated with cataracts |
| 🔴 Uveitis | Eye images associated with uveitis |
| ↔️ Crossed Eyes | Images showing crossed-eye appearance |
| 👀 Bulging Eyes | Images showing bulging-eye appearance |

*Classification performance depends on the training data and image quality. The model's output is not a confirmed diagnosis.*

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| 🐍 Python | Core programming language |
| ⚡ Fastai / Fastcore | Model training and deep learning utilities |
| 🔥 PyTorch | Deep learning framework |
| 🖼️ Pillow | Image processing |
| 🐼 Pandas | Data handling |
| 🔢 NumPy | Numerical operations |
| 📊 Matplotlib | Visualization and analysis |
| 🌐 Flask | Web application |
| 📓 Jupyter Notebook | Training and augmentation workflows |

---

## 🗂️ Project Structure

```text
EyeDiseaseDetection/
│
├── Original Dataset/
│   ├── Glaucoma/
│   ├── Cataracts/
│   ├── Uveitis/
│   ├── Crossed Eyes/
│   └── Bulging Eyes/
│
├── Augmented Dataset/
│   └── [Five class folders with augmented images]
│
├── augment_images.ipynb
├── model.ipynb
├── app.py
├── requirements.txt
├── eye_disease_model.pkl
└── README.md
```

*The dataset folders contain the original and augmented images. The trained model file must be present in the project root for the web app to run locally.*

---

## ⚙️ How It Works

```text
       📂 Eye Image Dataset
                │
                ▼
       🖼️ Image Augmentation
       Flips + 180° Rotations
                │
                ▼
       🧠 Fine-Tuned ResNet34
          Transfer Learning
                │
                ▼
       📊 Five-Class Prediction
                │
                ▼
          🌐 Flask Web App
```

1. **Dataset Preparation:** Organize eye images into five class-specific folders.
2. **Image Augmentation:** Generate flipped and rotated image copies to expand the training dataset.
3. **Model Training:** Fine-tune a pretrained ResNet34 model using Fastai and PyTorch.
4. **Model Export:** Save the trained model as `eye_disease_model.pkl`.
5. **Prediction:** Load the exported model in Flask to classify uploaded images.

---

## 📈 Model Training

- **Architecture:** ResNet34
- **Learning approach:** Transfer learning with fine-tuning
- **Training duration:** 50 epochs
- **Training data:** Augmented eye disease image dataset
- **Output:** Five-class image classification model

For detailed training results, visualizations, and implementation details, refer to `model.ipynb`.

*Accuracy, precision, recall, and other performance metrics should be added here only after verifying the actual notebook results.*

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/sillysaad/EyeDiseaseDetection.git
cd EyeDiseaseDetection
```

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv venv
```

Activate it:

**Windows**
```bash
venv\Scripts\activate
```

**Linux / macOS**
```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Run the Web Application

Ensure `eye_disease_model.pkl` exists in the project root, then run:

```bash
python app.py
```

Open the local address configured by the Flask application, typically:

```text
http://127.0.0.1:5000
```

If your Flask application is configured to use HTTPS, use the corresponding HTTPS address instead. A temporary development certificate may trigger a browser warning.

---

## 🧪 Training the Model

To reproduce the training workflow:

1. Place the original images in `Original Dataset/`, organized by class.
2. Run `augment_images.ipynb` to generate augmented images if required.
3. Ensure the five class folders are available in `Augmented Dataset/`.
4. Open `model.ipynb` and update the dataset path for your system.
5. Execute the notebook cells to train and fine-tune ResNet34.
6. Export the trained model as `eye_disease_model.pkl`.
7. Place the exported model in the project root before starting the Flask application.

---

## 🔮 Future Improvements

- 📊 Add verified evaluation metrics and a confusion matrix.
- 🎯 Improve generalization through dataset validation and careful augmentation.
- 📱 Enhance the interface for mobile and desktop users.
- ⚡ Optimize inference speed and model deployment.
- 🧾 Display prediction confidence with appropriate limitations.
- 🩺 Evaluate the model on independent, clinically validated datasets.

---

## 👨‍💻 Author

Saaduddin Shaikh - 
Developed as a deep learning project exploring computer vision, transfer learning, image augmentation, and web deployment.

<p align="center">
  <a href="https://web-production-1a232.up.railway.app/">
    <img src="https://img.shields.io/badge/🌐_Explore_the_Live_Project-Visit_Now-6C63FF?style=for-the-badge" alt="Explore Live Project"/>
  </a>
</p>
<img width="1914" height="944" alt="image" src="https://github.com/user-attachments/assets/8c837ff0-af46-4e3a-80bc-a1c143c72c98" />

---

<p align="center">
  ⭐ If you find this project interesting, consider giving the repository a star!
</p>

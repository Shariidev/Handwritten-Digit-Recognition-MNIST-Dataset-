# ✍️ Handwritten Digit Recognition using CNN (MNIST)

## 📌 Project Overview

This project builds a **Convolutional Neural Network (CNN)** to recognize handwritten digits (0–9) using the famous **MNIST dataset**.
The model is inspired by the classic **LeNet architecture** and is implemented using **PyTorch**.

It can:

* Train on handwritten digit images
* Predict digits from new images
* Save and load trained model weights

---

## 🧠 Model Architecture

The CNN consists of:

* Convolution Layer → ReLU → Average Pooling
* Convolution Layer → ReLU → Average Pooling
* Fully Connected Layer → ReLU
* Fully Connected Layer → ReLU
* Output Layer (10 classes)

This structure helps the model learn image patterns effectively.

---

## 📂 Project Structure

```
Handwritten-Digit-Recognition-MNIST-Dataset-
│
├── lenet.pth                # Trained model weights
├── train.ipynb              # Google Colab training notebook
├── requirements.txt        # Required libraries
└── README.md               # Project documentation
```

---

## ⚙️ Technologies Used

* Python
* PyTorch
* Torchvision
* NumPy
* Matplotlib
* PIL (Python Imaging Library)
* Scikit-learn

---

## 🚀 How to Run the Project

### 1️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 2️⃣ Train the Model

Run the notebook:

```
train.ipynb
```

### 3️⃣ Load Saved Model

```python
model.load_state_dict(torch.load("lenet.pth"))
model.eval()
```

### 4️⃣ Make Predictions

The model can predict digits from external images after preprocessing.

---

## 📊 Dataset

The MNIST dataset contains:

* 60,000 training images
* 10,000 testing images
* Grayscale images (28×28 pixels)

---

## 🎯 Results

The model achieves high accuracy on validation data and correctly predicts unseen handwritten digits.

Example:

```
Predicted Digit: 5
Confidence: 100%
```

---

## 💾 Model File

`lenet.pth` contains the trained weights and can be reused without retraining.

---

## ✨ Future Improvements

* Add GUI for drawing digits
* Deploy as web app
* Try deeper CNN architectures
* Hyperparameter tuning

---

## 👩‍💻 Author

**Sharanya (Shariidev)**

---

## 📜 License

This project is for educational and learning purposes.

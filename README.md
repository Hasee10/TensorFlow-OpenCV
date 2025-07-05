# 🧠 Streamlit + OpenCV + ML App

This project is a **web-based machine learning application** built using **Streamlit**, **OpenCV**, and optionally **TensorFlow**/**PyTorch**. It provides an interactive interface for image processing and classification tasks using modern computer vision models like **MobileNetV2**.

---

## 📌 Table of Contents

- [📌 Table of Contents](#-table-of-contents)
- [✨ Features](#-features)
- [📁 Project Structure](#-project-structure)
- [⚙️ Requirements](#️-requirements)
- [📦 Installation](#-installation)
- [🚀 Running the App](#-running-the-app)
- [🔍 How It Works](#-how-it-works)
- [📸 Example Use Cases](#-example-use-cases)
- [📌 Troubleshooting](#-troubleshooting)
- [📜 License](#-license)
- [🤝 Acknowledgements](#-acknowledgements)

---

## ✨ Features

- ✅ Image Upload and Preview
- ✅ Real-time image classification using MobileNetV2
- ✅ Streamlit web interface for easy use
- ✅ Webcam capture and OpenCV integration
- ✅ Works offline in a virtual environment
- ✅ Cross-platform (tested on Windows)

---

## 📁 Project Structure

```bash
Python_Project_2/
│
├── .venv/                   # Virtual environment folder (auto-managed by uv)
├── main.py                  # Main Streamlit application
├── requirements.txt         # Locked package versions
├── README.md                # This file
└── assets/                  # Optional: images, sample input, etc.
````

---

## ⚙️ Requirements

> ✅ These tools must be installed before using the app.

* Python 3.12 (or lower)
* [UV (Universal Virtualenv)](https://github.com/astral-sh/uv)
* (Optional) Git for version control

---

## 📦 Installation

### 🧪 Step-by-Step (Windows)

#### 1. ✅ Clone or download this repo

```bash
git clone https://github.com/yourusername/Python_Project_2.git
cd Python_Project_2
```

Or manually download and extract the ZIP.

---

#### 2. ✅ Initialize project with `uv`

```bash
uv init .
```

---

#### 3. ✅ Add dependencies (choose one):

### Option A: With PyTorch (recommended for Python 3.13)

```bash
uv add streamlit opencv-python torch torchvision --link-mode=copy --no-cache
```

### Option B: With TensorFlow (only works with Python ≤ 3.12)

```bash
uv add streamlit opencv-python tensorflow --link-mode=copy --no-cache
```

---

## 🚀 Running the App

### Step 1: Activate the virtual environment

```bash
.venv\Scripts\activate
```

### Step 2: Launch Streamlit

```bash
streamlit run main.py
```

> A local web browser window will open at `http://localhost:8501/`.

---

## 🔍 How It Works

* The app uses `Streamlit` to create a web interface.
* Users can:

  * Upload or capture images using webcam
  * See real-time predictions using MobileNetV2
  * Apply OpenCV filters if needed
* Models are loaded from either:

  * `torchvision.models.mobilenet_v2(pretrained=True)`
  * or `tensorflow.keras.applications.MobileNetV2` (if using TensorFlow)

---

## 📸 Example Use Cases

* 🐶 Classifying images of animals or objects
* 👁️ Real-time webcam detection
* 🖼️ Edge detection, color filtering using OpenCV
* 📱 Building mobile-friendly ML demos

---

## 📌 Troubleshooting

| Issue                       | Solution                                                  |
| --------------------------- | --------------------------------------------------------- |
| `ModuleNotFoundError`       | Run `uv add <package>` inside project folder              |
| `.DS_Store: os error 32`    | Run with `--link-mode=copy --no-cache`                    |
| TensorFlow fails to install | Use Python 3.12 or switch to PyTorch                      |
| OneDrive permission errors  | Move project to `C:\PythonProjects\YourAppName`           |
| Web app not loading         | Make sure no firewall or VPN is blocking `localhost:8501` |

---

## 📜 License

This project is licensed under the [MIT License](LICENSE) — feel free to use, modify, and distribute it.

---

## 🤝 Acknowledgements

* [Streamlit](https://streamlit.io/)
* [OpenCV](https://opencv.org/)
* [PyTorch](https://pytorch.org/)
* [TensorFlow](https://tensorflow.org/)
* [UV Package Manager](https://github.com/astral-sh/uv)

---

*Developed with 💻 by Muhammad Haseeb*

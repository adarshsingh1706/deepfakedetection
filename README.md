# Deepfake Detection using Generative AI and Grad-CAM 🔍🤖

This project detects **deepfake images** using a custom-trained `InceptionResnetV1` model (based on FaceNet) and visualizes the model’s decision with **Grad-CAM**. It includes a Gradio-powered web UI for real-time testing and demonstration.

---

## 🚀 Features

- 📸 Face detection using **MTCNN**
- 🧠 Deepfake classification using **InceptionResnetV1**
- 🔥 Heatmap visualization with **Grad-CAM**
- 🖼️ Web interface built with **Gradio**
- 🛠️ Code optimized for both **CPU and GPU**

---

## 🛠️ Tech Stack

- Python 3.x
- [PyTorch](https://pytorch.org/)
- [facenet-pytorch](https://github.com/timesler/facenet-pytorch)
- [Grad-CAM](https://github.com/jacobgil/pytorch-grad-cam)
- [Gradio](https://www.gradio.app/)
- OpenCV, PIL, NumPy

---

## 🧩 Model Info

We use a **custom-trained** `InceptionResnetV1` model:
- Pretrained on `vggface2`
- Fine-tuned for binary classification: **real** vs **fake**
- Output layer: Sigmoid (threshold at 0.5)

Due to GitHub’s 100MB limit, the model `.pth` file is **not included** in the repo.

🔗 [Upload your model file separately or use a download link]

---

## 📦 Installation

```bash
git clone https://github.com/adarshsingh1706/deepfakedetection.git
cd deepfakedetection

# (Optional) Create a virtual environment
python -m venv venv
venv\Scripts\activate   # On Windows
# or
source venv/bin/activate  # On Linux/macOS

pip install -r requirements.txt

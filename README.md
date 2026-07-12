# 👨‍👩‍👧 Family Face Recognition System

A real-time face recognition system that identifies family members through a webcam and displays their name and relation (e.g., **"Ali (Father)"**). The project uses **PyTorch** for deep learning and **OpenCV** for face detection.

---

## 🚀 Features

- Real-time face detection using OpenCV Haar Cascades
- Face classification with ResNet-18 (Transfer Learning)
- Displays the detected person's name and relation
- Custom dataset of family member images
- Model evaluation using Precision, Recall, and Accuracy
- Live webcam-based recognition
- Fast and lightweight implementation

---

## 📂 Project Structure

```text
FACE_RECOGNITION_OF_FAMILY_MEMBERS/
│
├── dataset/
│   ├── train/
│   │   ├── ali/
│   │   ├── fathima/
│   │   └── sajeela/
│   │
│   └── val/
│       ├── ali/
│       ├── fathima/
│       └── sajeela/
│
├── train_model.py          # Model training script
├── realtime_face.py        # Real-time face recognition
├── face_model.pth          # Trained model
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/your-username/family-face-recognition.git

cd family-face-recognition
```

### Create a virtual environment

```bash
python -m venv venv
```

### Activate the environment

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

### Install dependencies

```bash
pip install torch torchvision opencv-python pillow
```

---

## 📁 Prepare the Dataset

Place images inside the following folders:

```text
dataset/
├── train/
│   ├── ali/
│   ├── fathima/
│   └── sajeela/
│
└── val/
    ├── ali/
    ├── fathima/
    └── sajeela/
```

Each folder should contain multiple images of the corresponding family member.

---

## 🏋️ Training the Model

Run the training script:

```bash
python train_model.py
```

The script will:

- Load the training and validation datasets
- Fine-tune a pretrained ResNet-18 model
- Save the trained model as **face_model.pth**

---

## 🎥 Real-Time Recognition

Run the recognition script:

```bash
python realtime_face.py
```

The application will:

- Open the webcam
- Detect faces using OpenCV Haar Cascades
- Recognize family members
- Display the person's name and relationship on the video feed

Press **q** to exit the application.

---

## 📊 Results

| Metric | Value |
|---------|-------|
| Precision | 94.8% |
| Recall | 93.9% |
| Accuracy | 95.3% |

---

## 🛠️ Technologies Used

- Python
- PyTorch
- torchvision
- ResNet-18 (Transfer Learning)
- OpenCV
- Pillow (PIL)

---

## 📖 Future Improvements

- Expand the dataset with additional family members
- Replace Haar Cascades with MTCNN or dlib for improved face detection
- Apply data augmentation techniques to improve model performance
- Deploy the application as a desktop or mobile application
- Add face registration for new family members
- Integrate cloud-based face recognition support

---

## 👩‍💻 Author

**Farha C Ali**  
**B.Tech Artificial Intelligence & Data Science**

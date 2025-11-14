# 🖊️ IntelliBoard – AI-Powered Whiteboard

IntelliBoard is an interactive AI-powered whiteboard web app built using **React** (frontend) and **Flask** (backend) with Firebase integration.  
It allows users to draw freely, erase, select tools, and use AI features like text recognition (OCR), image captioning, and automatic summarization.

---

## 🌟 Features

- 🖌️ **Drawing Tools**
  - Pencil, Brush, Highlighter, Shapes (Line, Rectangle, Circle)
  - Adjustable size and color palette
  - Eraser and Clear Canvas option

- 🧠 **AI Tools**
  - Handwritten text → Typed text (TroCR OCR)
  - Auto-caption generation for images
  - Slide summary creation

- 🪄 **Utility Features**
  - Add new slides
  - Save whiteboard as `.png` or `.pdf`
  - Export and load saved slides

- ☁️ **Backend & Storage**
  - Flask backend with AI model pipeline
  - Firebase for authentication and file storage

---

## 🧰 Tech Stack

| Layer | Technologies |
|-------|---------------|
| **Frontend** | React.js, HTML5 Canvas, CSS3, JavaScript |
| **Backend** | Python Flask, PyTorch, Transformers, OpenCV |
| **AI Models** | [Microsoft TroCR](https://huggingface.co/microsoft/trocr-base-stage1), Image Captioning (BLIP / ViT-GPT2) |
| **Database / Auth** | Firebase |
| **Deployment (optional)** | GitHub Pages / Render / Firebase Hosting |

---

## ⚙️ Project Setup

### 1️⃣ Clone the Repository

git clone https://github.com/Abhinav-dev25/Whiteboard.git
cd Whiteboard

2️⃣ Setup the Backend (Flask)

### Create and Activate Virtual Environment
python -m venv .venv
.venv\Scripts\activate       # On Windows


### Install Dependencies
pip install -r requirements.txt

### Run Flask Server
cd backend
python app.py
The Flask server will start at http://127.0.0.1:5000

3️⃣ Setup the Frontend (React)

cd frontend
npm install
npm start
The React app will run on http://localhost:3000

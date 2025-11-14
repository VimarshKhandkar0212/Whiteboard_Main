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

Backend:
ml_models:
  captions.py: https://drive.google.com/file/d/1h5s_01Vppbdkug6Rwf1wjT4g0C3VnnaU/view?usp=sharing   
                            fine_tune_bart.py file: https://drive.google.com/file/d/16WzDagBPXX2xHkpPSyFf2UPWDkfbhBun/view?usp=sharing   
                            fine_tune_trocr.py file: https://drive.google.com/file/d/1Qrmn_sotPxV7D0pLrrM6RKt5XpFoS-GU/view?usp=sharing   
                            fine_tune_vitgpt2.py file: https://drive.google.com/file/d/1mVLlbIS8pU7uMUW3R1KHGg1UegQrVRjH/view?usp=sharing   
                            summarizer.py: https://drive.google.com/file/d/1uxwqFVGZlbolQaBVJ5or_Y1WlUb07PKq/view?usp=sharing  
                            trOCR.py: https://drive.google.com/file/d/1gcy4kSlswkBqgvLfLI0KyjjS-ixlCMw1/view?usp=sharing  
                            app.py: https://drive.google.com/file/d/1P-_hTzC32wBATDB9wWYtKZ5a10E9omH6/view?usp=sharing  
                            config.py: https://drive.google.com/file/d/1dl_0vC20_NkLRa-Rsuy_fb4Xh9U2mKul/view?usp=sharing  
Frontend:
                            src:  
                            {components:   
                            PreviewPanel.jsx: https://drive.google.com/file/d/1iyF0JQL8FumljjKHJHdR_w4NPDp8VgJq/view?usp=sharing  
                            SlidesPanel.jsx: https://drive.google.com/file/d/1eZjfqYgxF6g-jdZDxDVHkKSe78gLEeZ2/view?usp=sharing  
                            Toolbar.jsx: https://drive.google.com/file/d/1tiqLa3H-8t4eRudX1GF6Nk2RKa-scosD/view?usp=sharing  
                            Whiteboard.jsx: https://drive.google.com/file/d/1tiqLa3H-8t4eRudX1GF6Nk2RKa-scosD/view?usp=sharing }  
                            api.js: https://drive.google.com/file/d/1jlIqNbMB-vuYSPnf8GWlIC769wQEGsy8/view?usp=sharing  
                            app.jsx: https://drive.google.com/file/d/1q0MfQLTmao2hdurDOfuJEcjFNrCP0cgs/view?usp=sharing  
                            main.jsx: https://drive.google.com/file/d/1wub2CRuhvd7di1BTj6wVLpZvhefjW3KI/view?usp=sharing  
                            styles.css: https://drive.google.com/file/d/17Y56kJIgHCDK1865Ayu3wnAlFS6Wvnhm/view?usp=sharing  

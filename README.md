# MathScribe-OCR

### Printed Mathematical Expression Recognition & LaTeX Conversion System

MathScribe-OCR is a full-stack system for converting images of **printed mathematical expressions** into structured **LaTeX code**.

The project combines a Pix2TeX-based OCR backend with an interactive web interface for uploading mathematical expressions, generating LaTeX transcriptions, and previewing the resulting output.

## 🎯 Project Goal

Mathematical expressions contain complex spatial relationships such as fractions, superscripts, integrals, matrices, and operator alignment that cannot be handled effectively through basic character-level OCR.

MathScribe-OCR explores a structured image-to-LaTeX approach designed to:

- Recognize printed mathematical expressions
- Convert mathematical notation into LaTeX
- Preserve the structural relationships between symbols
- Provide an interface for reviewing and displaying generated results

## 🏗️ System Architecture

The system consists of two main components:

### Frontend

Built with **React, Vite, and Tailwind CSS**.

The interface supports:

- Mathematical expression image upload
- Generated LaTeX display
- Rendered formula preview
- Interactive result handling

### Backend

Built with **FastAPI** and a mathematical OCR model.

The backend handles:

- Image processing
- OCR inference
- Mathematical expression transcription
- LaTeX generation
- API communication with the frontend

## 🧠 OCR Model

The backend uses **Pix2TeX (LaTeX-OCR)**, an open-source image-to-LaTeX model designed for mathematical expression recognition.

Model reference:

https://github.com/lukas-blecher/LaTeX-OCR

## 🔄 Workflow

1. The user uploads an image containing a printed mathematical expression.
2. The frontend sends the image to the backend.
3. The OCR model processes the mathematical notation.
4. The expression is converted into LaTeX.
5. The generated result is returned to the interface for display and review.

## 🛠️ Technologies

**Frontend**
- React
- Vite
- Tailwind CSS
- TypeScript

**Backend**
- Python
- FastAPI
- Pix2TeX / LaTeX-OCR

**AI / Computer Vision**
- Mathematical OCR
- Image-to-LaTeX
- Deep Learning
- Computer Vision

## 📁 Project Structure

```text
MathScribe-OCR1/
│
├── frontend/
├── Backend/
├── README.md
└── .gitignore
```

## ▶️ Running the Project

Both the backend and frontend must be running for the complete system to work.

### Backend

Navigate to the backend directory:

```bash
cd Backend
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

If compatibility issues occur with NumPy 2.x:

```bash
pip uninstall numpy -y
pip install "numpy<2"
pip install -r requirements.txt
```

Start the backend:

```bash
python server.py
```

### Frontend

Navigate to the frontend directory:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

The frontend will then be available locally.

## 👥 Project Contributors

MathScribe-OCR was developed as a team project by:

- Maram Moshabbab Al Romman
- Lama Muidh Alsulami
- Rimas Yasir Allehaibi
- Layan Munwer Almoqati
- Lama Mousa Alzahrani

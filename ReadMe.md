
# 🎞️ LectureCapture

> Automatically extract meaningful lecture slides from YouTube videos using AI and generate a clean PDF.  
> Save time, skip screenshots, and get organized notes with a single click.

---

## 📌 Features

- 🎥 Download lectures directly from YouTube
- 🧠 Detect and extract **unique slides** using deep frame comparison
- 🔍 Integrated **OCR** for reading slide content
- 📄 Auto-generate a clean **PDF** of extracted slides
- 🖼️ GUI built with **Tkinter**
- 📊 Progress bar with real-time updates
- 🧵 Threaded download & extraction (non-blocking)

---

## 🧰 Built With

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![Tkinter](https://img.shields.io/badge/Tkinter-black?logo=python&logoColor=white) ![Pillow](https://img.shields.io/badge/Pillow-cc6699?logo=python&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-27338e?logo=opencv&logoColor=white) ![Tesseract OCR](https://img.shields.io/badge/TesseractOCR-35495E?logo=tesseract&logoColor=white) ![ReportLab](https://img.shields.io/badge/reportlab-FF6F00?logo=adobeacrobatreader&logoColor=white) ![yt-dlp](https://img.shields.io/badge/yt--dlp-blue?logo=youtube&logoColor=white)
---

## 📂 Project Structure

```
LectureCapture/
│
├── slide_extractor.py       # Core logic for detecting unique slides
├── app.py                   # Tkinter GUI interface
├── requirements.txt         # All dependencies
├── output/                  # Folder for storing extracted slides and final PDF
└── README.md
```

---

## ⚙️ Setup Instructions

1. Clone or download the repository to your local machine:
   ```bash
   git clone https://github.com/divA2805/LectureCapture.git
   cd LectureCapture
   ```

2. Make sure the `slide_extractor.py` file is in the same directory as `app.py` or correctly referenced.

---

## 🚀 Getting Started

### 1️⃣ Install Dependencies

Make sure you have Python ≥ 3.8 installed.

```bash
pip install -r requirements.txt
```

Also, install Tesseract OCR:

- **Windows**: [Tesseract Installer](https://github.com/tesseract-ocr/tesseract/wiki)
- **Ubuntu**:

```bash
sudo apt install tesseract-ocr
```

---

### 2️⃣ Run the App

```bash
python app.py
```

A GUI will open where you can:

- Paste the YouTube link  
- Choose a download location  
- Click "Start" to begin download, slide extraction, and PDF generation

---

## 🧠 How It Works

- The video is downloaded using `yt-dlp`
- Frames are sampled at intervals
- Similar or duplicate frames are removed using OpenCV comparison
- OCR reads any visible slide text (optional, for enhancements)
- Final slides are compiled into a professional PDF using ReportLab

---

## 📸 Sample Output

> ✅ Clean slides PDF from a 1-hour technical lecture in under 2 minutes  
> 📁 Slides saved in `output/` with timestamped filenames  
> 🧾 Final PDF available for download

---

## 🙋‍♂️ Author

Made with ❤️ 

---


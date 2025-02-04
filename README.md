# 🚗 Automatic Number Plate Recognition (ANPR) System

This project implements an **Automatic Number Plate Recognition (ANPR)** system using **OpenCV** and **Tesseract OCR**. The system captures an image from a webcam, detects the vehicle's number plate, extracts the text using Optical Character Recognition (OCR), and saves the results in an **Excel spreadsheet**.

---

## 📌 Features

✅ **Real-time Image Capture** – Captures a frame from the webcam
✅ **Image Preprocessing** – Uses grayscale conversion, filtering, and edge detection
✅ **Number Plate Detection** – Detects number plates based on contours and bounding boxes
✅ **OCR Processing** – Extracts text from the detected plate using **Tesseract OCR**
✅ **Excel Storage** – Saves extracted text in an Excel file for record-keeping

---

## 🏗️ Tech Stack

| Component       | Technology Used |
|----------------|----------------|
| Programming Language | Python |
| Image Processing | OpenCV, Imutils |
| OCR | Tesseract |
| Data Handling | Pandas, OpenPyXL |
| GUI | Command Line |

---

## 📂 Project Structure

```
ANPR_Project/
│── anprorg2.py       # Main Python script
│── captured_plate.jpg # Captured image from webcam
│── number_plate.png   # Cropped detected number plate image
│── anpr_output.xlsx   # Output file storing detected plate numbers
│── README.md          # Project documentation
```

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-repo/anpr.git
cd anpr
```

### 2️⃣ Install Dependencies
```bash
pip install opencv-python imutils pytesseract pandas openpyxl
```

### 3️⃣ Configure Tesseract OCR
📌 **Ensure Tesseract is installed on your system**. You can download it from:
[Tesseract OCR Download](https://github.com/UB-Mannheim/tesseract/wiki)

Then, update the path to the **Tesseract executable** in `anprorg2.py`:
```python
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
```

### 4️⃣ Run the Application
```bash
python anprorg2.py
```

---

## 🎯 How It Works

1️⃣ **Captures an image** from the webcam when you press 'q'  
2️⃣ **Preprocesses the image** (grayscale, edge detection, noise filtering)  
3️⃣ **Detects the number plate** based on contour approximation  
4️⃣ **Extracts text** from the detected plate using OCR  
5️⃣ **Saves the detected number** plate text into an Excel file  

---

## 📊 Sample Output

**Detected Text:** `ABC1234`

**Excel Output:**
| Detected Text | Cleaned Text |
|--------------|-------------|
| ABC1234 | ABC1234 |

---

## 📜 License

👤  This project is **open-source**. Feel free to modify and improve it!  


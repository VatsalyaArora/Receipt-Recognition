# 🧾 AI Receipt Scanner & Data Extractor
**A specialized OCR pipeline for digitizing financial documents with custom image pre-processing.**

## 📌 Project Overview
This project automates the extraction of structured data from physical receipts. Unlike standard OCR, this system utilizes a custom computer vision pipeline to handle common real-world issues such as skewed text, shadows, and low contrast, achieving high-accuracy data extraction for financial logging.

## 🛠️ Technical Architecture
- **OCR Engine:** Tesseract / EasyOCR (customizable).
- **Computer Vision:** OpenCV for advanced pre-processing.
- **Data Structuring:** Regular Expressions (Regex) for extracting Totals, Dates, and Merchant names.
- **Language:** Python 3.10+.

## 🚀 Key Features
- **Custom Pre-processing:** Implements grayscale conversion, Gaussian blurring, and Otsu's Thresholding to reduce noise.
- **Perspective Correction:** (If implemented) Automatically detects receipt edges and "flattens" the image.
- **Noise Reduction:** Specialized filters to handle "noisy" backgrounds and wrinkled paper.
- **Structured Output:** Converts raw text into a clean JSON format or CSV for accounting software.

## 📈 Performance Highlights
- Developed custom pre-processing pipelines specifically for **grayscale and skew correction**.
- Optimized to handle low-light mobile photos of receipts.

## Required
- Have a image by the name of "receipt.jpg"

## 📦 Installation
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/vatsalya-arora/Receipt-Recognition.git](https://github.com/vatsalya-arora/Receipt-Recognition.git)
2.  **Install Dependencies:**
   ```bash
   pip install opencv-python pytesseract numpy
3.  **Run the Scanner:**
   ```bash
   python main.py --image path/to/receipt.jpg

# 🏗️ Project Structure
src/preprocessing.py: Image cleaning logic (thresholding, denoising).
src/extractor.py: OCR and Regex parsing logic.
data/samples/: Example receipts for testing.
output/: Extracted data in JSON/CSV format.

# 🎓 About
Developed by Vatsalya Arora as part of a portfolio in AI and Computer Vision, focusing on practical data cleaning and noise reduction techniques.

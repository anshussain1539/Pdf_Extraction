# PDF Image Extraction and OCR

This project extracts images from each page of a PDF file and performs Optical Character Recognition (OCR) on those images using Tesseract OCR to convert them into text.

## Requirements

- Python 3.x
- [PyMuPDF (fitz)](https://pymupdf.readthedocs.io/en/latest/)
- [Pillow](https://pillow.readthedocs.io/en/stable/)
- [pytesseract](https://pypi.org/project/pytesseract/)

## Installation

1. **Install the required Python libraries:**

   ```sh
   pip install PyMuPDF pillow pytesseract
   ```

2. **Install Tesseract OCR:**

   - **Windows:**
     1. Download the Tesseract OCR installer from the [official repository](https://github.com/tesseract-ocr/tesseract).
     2. Run the installer and follow the setup instructions.
     3. Note the installation path (usually `C:\Program Files (x86)\Tesseract-OCR\tesseract.exe`).

   
## Usage

1. **Set the Tesseract executable path:**
   ```python
   pytesseract.pytesseract.tesseract_cmd = r'C:\\Program Files (x86)\\Tesseract-OCR\\tesseract.exe'  # Update this path if necessary
   ```

2. **Open and process the PDF:**
   - Place your PDF file in the same directory as the script or provide the full path to the PDF file.
   - Update the `pdf_path` variable with your PDF file name or path.

3. **Run the script:**
    - The File which is uploaded.
      
## Notes

- Ensure that the `tesseract_cmd` path is correctly set to the location of your Tesseract executable.
- The script assumes one image per page in the PDF. Adjust as necessary if your PDF contains multiple images per page.

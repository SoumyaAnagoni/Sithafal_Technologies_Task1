# Sithafal_Technologies_Task1
# PDF Processing Tool

This repository contains a Python script to extract text, tables, and images from specific pages of a PDF file. It uses pdfplumber for text and table extraction and PyMuPDF (fitz) for image extraction.

## Features

- Extracts text and tables from specified PDF pages.
- Extracts images from specified PDF pages and saves them in a designated output directory.
- Handles user queries to specify pages dynamically.

## Requirements

Ensure you have Python installed, then install the necessary dependencies:

bash
pip install --upgrade pymupdf pdfplumber


## Usage

1. Clone the repository:
   bash
   git clone https://github.com/SoumyaAnagoni/pdf-processing-tool.git
   cd pdf-processing-tool
   

2. Prepare your environment:
   - Place the PDF file in the desired directory.
   - Update the script with the path to your PDF file and the output directory for images.

3. Run the script:
   bash
   python pdf_processing.py
   

4. Enter your query when prompted:
   - Specify pages in the format page 1 page 3.
   - The script will process the requested pages, extracting text, tables, and images.

## Example

For a PDF located at /content/Sitafal/sithafal file.pdf, you can run:

plaintext
Enter your query: page 1 page 3


Output:
- Text and tables will be displayed in the console.
- Extracted images will be saved in the /content/output/ directory.

## Script Overview

### Functions

1. **extract_text_and_tables(pdf_path, page_number)**:
   - Extracts text and tables from a specified page using pdfplumber.

2. **extract_images(pdf_path, page_number, image_output_dir)**:
   - Extracts images from a specified page using PyMuPDF and saves them to the output directory.

3. **handle_query(user_query, pdf_path, image_output_dir)**:
   - Processes user queries to extract data from specified pages.

### Input
- pdf_path: Path to the PDF file.
- image_output_dir: Directory to save extracted images.
- user_query: Query specifying the pages to process (e.g., page 1 page 3).

### Output
- Console output with extracted text and table data.
- Saved images in the specified output directory.

## Directory Structure


project-root/
│
├── pdf_processing.py      # Main script for PDF processing
├── README.md              # Documentation
├── requirements.txt       # List of dependencies
└── static/                # Directory for storing extracted images


## Improvements

### Future Enhancements
- Support for page ranges (e.g., page 1-3).
- Output results to a text file or JSON format.
- Multithreading for processing large PDFs efficiently.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contributions

Contributions are welcome! Please open an issue or submit a pull request for any improvements or features.

---

Feel free to contact me for questions or feedback!

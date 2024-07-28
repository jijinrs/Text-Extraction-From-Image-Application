# Text Extraction from Image Application
This project is a Flask-based web application that performs Optical Character Recognition (OCR) to extract text from images using Tesseract OCR.

## Features
Upload images and extract text
Display extracted text on the web interface
Simple and user-friendly interface

## Prerequisites
Python 3.8
opencv-python-headless==4.2.0.32
pytesseract==0.3.7
numpy==1.19.3
Pillow==8.0.1
itsdangerous==1.1.0
Flask==1.1.2
Werkzeug==0.16.1

## Installation
Follow these steps to set up and run the application locally.

## Step 1: Clone the Repository
### Clone the project repository from GitHub.
   git clone https://github.com/jijinrs/Text-Extraction-From-Image-Application.git
   cd Text-Extraction-From-Image-Application

## Step 2: Create and Activate Virtual Environment
   Create and activate a virtual environment using Conda.
   conda create --name ocr_env python=3.8
   conda activate ocr_env

## Step 3: Install Dependencies
  Install the required dependencies from the requirements.txt file.
  pip install -r requirements.txt

## Step 4: Install Tesseract OCR
   Download and install Tesseract OCR from this link.
   Note the installation path. The default installation path is C:\Program Files\Tesseract-OCR.

## Step 5: Configure Tesseract Path
   Update the Tesseract command path in your code. Open the Python file where Tesseract is configured (typically in the main application file or a configuration file) and set the Tesseract path.
   pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'
## Step 6: Run the Application
   Start the Flask application.
   python app.py
   
## Step 7: Access the Application
Open your web browser and go to http://127.0.0.1:5000 to access the application.

## Step 8: Test the Application
 Upload an image using the web interface and see the extracted text displayed.

Folder Structure
Text Extraction from Image Application/
│
├── app/
│ ├── init.py
│ ├── views.py
│ ├── static/
│ │ ├── css/
│ │ ├── images/
│ │ └── js/
│ └── templates/
│ └── index.html
│
├── sample_data/
│ └── example.jpg
│
├── .gitignore
├── README.md
├── requirements.txt
└── app.py
## Troubleshooting
  TesseractNotFoundError: Ensure that Tesseract is installed and the path is correctly set.
  ImportError: Ensure all dependencies are installed using pip install -r requirements.txt.
Contributing
Feel free to contribute by submitting a pull request or opening an issue.

License
This project is licensed under the MIT License.

By following the above instructions, you should be able to set up and run your OCR application locally. If you have any issues, feel free to open an issue on the repository.

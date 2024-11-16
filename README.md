# Creditsafe-Application

## Description
This Jupyter Notebook uses a combination of OCR, computer vision techniques, regex, and generative AI to provide a general-purpose solution to the problem of scanning multilingual documents in English, French, Dutch, or German from the Belgian Gazette Service and extracting information from the text therein.

### Assumptions
Several key assumptions have been made from observations on the supplied sample data set about the layout of the documents, which it is assumed is approximately the same throughout different languages and types of documents. This layout assumption is summarized in the following image:
![Layout Diagram](https://github.com/franna-cotta/creditsafe-application/blob/main/images/Layout_Example.jpg)
- Red: Border region, ignored and cropped out
- Blue: Upper text headers
- Green: Upper text
- Cyan: Middle text headers
- Pink: Middle text
- Yellow: Lower (body) text

## Requirements
This notebook requires Jupyter Notebook, Python 3.10+, Ghostscript, Tesseract OCR all to be installed on the local machine.
- Jupyter Notebook (https://jupyter.org/)
- Python (https://www.python.org/)
- Ghostscript (https://www.ghostscript.com/)
- Tesseract OCR (https://github.com/tesseract-ocr/tesseract)

## Running

# Creditsafe-Application

## Description
This Jupyter Notebook uses a combination of OCR, computer vision techniques, regex, and generative AI to provide a general-purpose solution to the problem of scanning multilingual documents in English, French, Dutch, or German from the Belgian Gazette Service and extracting information from the text therein.

### Data Assumptions
Several key assumptions have been made from observations on the supplied sample data set about the layout of the documents, described in the following image:

![Layout Diagram](https://github.com/franna-cotta/creditsafe-application/blob/main/images/Layout_Example.jpg)

- Red: Border region, (assumed) irrelevant
- Blue: Upper headers
- Green: Upper information
- Cyan: Middle header
- Pink: Middle information
- Yellow: Lower (body) text

It is assumed this style of layout is approximately the same throughout different languages and varieties of documents, and this assumption is used as the basis for the application of image processing techniques to isolate specific regions of text.

Other assumptions made include the existence of semicolons in the header regions, used to demarcate the separation between headers and information. The assumption that this is true for all of the headers in the blue region has not been made, as semicolon dividers were missing from the address section for several sample documents. However, it has been assumed they exist for at least *some* of the headers. The order of data in the upper headers and information section is also assumed to be fixed, independence of language and document type.

## Requirements
This notebook requires Jupyter Notebook, Python 3.10+, Ghostscript, Tesseract OCR all to be installed on the local machine.
- Jupyter Notebook (https://jupyter.org/)
- Python (https://www.python.org/)
- Ghostscript (https://www.ghostscript.com/)
- Tesseract OCR (https://github.com/tesseract-ocr/tesseract)
Additionally, an API Key for the Hugging Face platform (https://huggingface.co/) is required. The software will initially look for this under the *HUGGINGFACE_API_TOKEN* environment variable and will prompt the user for manual entry if this is not found.

## Running
To run the solution, open the main notebook with Jupyer and execute all the cells in sequential order using the command *Run -> Run All Cells*. Ensure

## Authors
- Francesca Carter (https://github.com/franna-cotta/)

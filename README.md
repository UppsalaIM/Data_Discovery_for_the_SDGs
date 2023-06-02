# Data_Discovery_for_the_SDGs

Source code and data for the paper "Data Discovery for the SDGs: A Systematic Rule-based Approach".

## Setup

You will need to install [Poppler](https://poppler.freedesktop.org/) and 
[Tesseract](https://tesseract-ocr.github.io/) before you can run the 
Python code.

Python requirements can be found in `requirements.txt`. 

## Usage

There are two Jupyter notebooks:
* `notebooks/01-Entity_Extraction.ipynb` : Loads PDFs from `data/sdg7-papers` 
(note: PDFs note included in this repository), converts each to 
images using Poppler, then uses Tesseract to perform OCR to extract the text, 
then extracts entities based on rules derived from `data/sdg7-coding-manual.xlsx` to output `sdg7-coding-auto.xlsx`.
* `notebooks/02-Plot_Figures.ipynb` : Loads `data/sdg7-coding-auto.xlsx` and 
applies some 
processing before plotting sunburst chart of data mapping distributions.



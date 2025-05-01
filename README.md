# Content-Based Image Retrieval (CBIR) Web

Tugas Besar 2 Aljambar Linier dan Geometri 

## Features

- **Dual Search Modes**: Search by color distribution or texture patterns
- **Interactive UI**: Simple drag-and-drop interface for image uploads
- **Dataset Management**: Upload and manage your own image collection
- **Real-time Results**: View similarity scores and execution time metrics
- **Responsive Design**: Works seamlessly across different devices

## Technologies

- **Backend**: Django 4.2+
- **Frontend**: HTML, CSS, Bootstrap 5
- **Image Processing**: NumPy, PIL (Python Imaging Library)
- **Database**: SQLite

## How It Works

### Color-Based Search
Converts images to HSV color space and generates histograms to compare color distributions between the query image and dataset. Similarity is calculated using cosine similarity.

### Texture-Based Search
Analyzes texture patterns using grayscale co-occurrence matrices. Extracts key features like contrast, homogeneity and entropy, then compares using normalized vectors.

## Getting Started

### Build With
- Python3
- Django
- Django-bootstrap
  ```
  pip install django-bootstrap-v5
  ```

### Installing Libraries
- NumPy
- PIL/Pillow

### Executing Program Through Website
1. Open the Terminal or Command Line
2. Clone this repo
   ```
   git clone https://github.com/ShafiqIrv/Algeo02-22003.git
   ```
3. Go to "Algeo02-003/src/cbir_web" directory
   ```
   cd Algeo02-003/src/cbir_web
   ```
4. Run this command
   ```
   py manage.py runserver
   ```
5. Hold "Ctrl" button and click the link to go to website page

## Usage Guide

1. Upload your image dataset using the "UPLOAD DATASET" button
2. Upload a query image using the "Insert Image Here" area
3. Select search mode (Color or Texture)
4. Click "Search" to find visually similar images
5. Browse through paginated results showing similarity percentages

## Project Structure

- `cbir_web/` - Main Django project
- `pages/` - Django app containing views, models, and templates
- `pages/static/` - Static files (CSS, JS, images)
- `pages/templates/` - HTML templates
- `pages/views.py` - Core CBIR implementation logic

## Authors

1. 13522003 - Shafiq Irvansyah
2. 13522005 - Ahmad Naufal Ramadan
3. 13522015 - Yusuf Ardian Sandi

# django-csv-analyzer
Web app for uploading, analyzing, and visualizing CSV files with Django.

# Features

- Upload CSV files for analysis.
- Display the first five rows of the data.
- Show summary statistics (mean, median, standard deviation) for numeric columns.
- Identify and handle missing values by dropping rows with missing values.
- Generate histograms for data visualization.

# Setup Instructions

Follow these steps to set up the project on your local machine:

# Prerequisites

- Python 
- Django
- Git
- pip

# Installation

1. Clone the Repository
   ```
   git clone https://github.com/ChadiBelhadj/Django-CSV-Analyzer.git
  ``
  

   cd csv-analyzer

3. Activate a Virtual Environment:
   use: venv\Scripts\activate



4. Install Dependencies:
   pip install -r requirements.txt
   This step will install all the required libraries in the project.

5. Run Migrations:
   python manage.py migrate

6. Run the Development Server:
   python manage.py runserver

7. Open the Application in Your Browser:
   - Navigate to `http://127.0.0.1:8000` in your web browser.

# Brief Explanation

This CSV Analyzer project consists of a Django application that provides a user interface for uploading CSV files, processing data, and visualizing the results.

# index.html:

The home page where users can upload CSV files.

# process.html:

Displays the first five rows of data, summary statistics, missing values, and handles missing values by dropping rows.

# visualize.html:

Displays histograms of the data.

The views in "views.py" handle the logic for reading CSV files, processing data, and generating visualizations. The "static/css/styles.css" file contains styles to improve the appearance of the web pages.

# Note:

- Ensure that the uploaded files are in CSV format.
- The project uses Matplotlib for generating histograms.

# BizCardX: Extracting Business Card Data with Optical Character Recognition (OCR)

## Introduction
Extracting business card data using Optical Character Recognition (OCR) is a cutting-edge solution for digitizing contact information from physical cards. With OCR technology, businesses can seamlessly convert printed text into digital formats, enabling easier integration into contact management systems and enhancing networking and customer relationship management efforts.

## Overview
This Streamlit web application enables users to upload images of business cards and extract essential information such as names, job titles, companies, contact details, and locations using easyOCR. Within the app, users can view, edit, or delete the extracted data. Additionally, the application allows users to save this information, along with the uploaded business card images, into a MySQL database that can store multiple entries, each associated with its respective image and details.

### 1. Tools Installed
* Visual Studio Code
* Jupyter Notebook
* Python 3.11.3 or later
* MySQL
  
### 2. Required Libraries
* streamlit, easyocr, cv2, mysql-connector-python, pandas, re, matplotlib.
 
### 3. Import Libraries
#### **Image handling libraries**
* import easyocr
* import cv2
#### **File handling libraries**
* import os
* import re
#### **SQL library**
* import mysql.connector as sql
#### **Pandas, Matplotlib**
* import pandas as pd
* import matplotlib.pyplot as plt  
#### **Dashboard libraries**
* import streamlit as st
* from streamlit_option_menu import option_menu
  
### 4. ETL and EDA Process
#### a) Data Extraction
* Extract the relevant data from business cards using easyocr.
#### b) Data Transformation
* After extraction, the obtained text data is organized into a structured format in the form of a dataframe.
#### c) Data Loading 
* The transformed data is then stored in the MySQL database in dataframe format.
#### d) Data Visualization, Update, and Deletion
* The extracted information can be visualized using matplotlib and displayed as a dataframe.
* Users can also update, modify, or delete data from the database.

## User Guide
#### Step 1. Home Tab
* This section offers a brief introduction to the project, outlining its features and the necessary tools.

#### Step 2. Upload and Extract Tab
* In this tab, users can browse for a business card image using the **Browse File** button and upload it in the **Upload Here** section. The application will process the image and extract the necessary data, displaying it alongside the processed image in text format.
* Users can upload the extracted data to MySQL by clicking the **Upload to MySQL** button. The data will be displayed in a dataframe.

#### Step 3. Modify Tab
* In this section, users can modify the data obtained from a business card, upload the updated information to the SQL database, and view the revised data.
* Users also have the option to delete records from the MySQL database as needed.

## YouTube video link:


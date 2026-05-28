# 🏡 Nigeria Property Market Data Pipeline & Pricing Intelligence System

##  Project Overview

This project is a Python-based web scraping and data engineering pipeline built to extract, clean, and structure real estate listings from NigeriaPropertyCentre across **Lagos, Abuja, and Port Harcourt**.

It covers multiple asset classes including **residential, commercial, retail, and land**, both for **sale and rent**, transforming unstructured property listings into structured market intelligence.

The final dataset is designed to support a real estate analytics platform that helps users understand pricing trends, compare locations, and make better investment decisions.

---

##  Objectives

- Scrape large-scale property listings across major Nigerian cities
- Extract structured data from unstructured HTML pages
- Capture key real estate attributes such as:
  - Property price
  - Location (city and district-level)
  - Asset class (Residential, Commercial, Retail, Land)
  - Sub-category (Duplex, Apartment, Office, Shop, Warehouse, etc.)
  - Listing type (For Sale / For Rent / Shortlet)
  - Property features (Bedrooms, Bathrooms, Toilets, Parking)
  - Listing date / update timestamp
- Build a structured dataset for analytics and dashboard development

---

##  Tech Stack

- Python 🐍
- BeautifulSoup (Web Scraping)
- Requests (HTTP handling)
- Pandas (Data processing & structuring)
- Regular Expressions (Data parsing & cleaning)
- OpenPyXL (Excel export)

---

##  How It Works

### 1. Web Scraping Engine
The script iterates through paginated listings on NigeriaPropertyCentre and sends HTTP requests to retrieve HTML content.

### 2. Data Extraction
Using BeautifulSoup, the scraper extracts:
- Property price
- Location (area-level data)
- Listing URL
- Property features (bedrooms, bathrooms, toilets, parking)
- Listing metadata from structured HTML and comments

### 3. Data Classification
Each property is automatically categorized into:

- **Category:** Residential, Commercial, Retail, Land  
- **Sub-category:** Duplex, Apartment, Office, Shop, Warehouse, etc.  
- **Offer Type:** Sale, Rent, Shortlet  

### 4. Data Structuring
All extracted data is stored in structured Python dictionaries and compiled into a Pandas DataFrame.

### 5. Export
Final dataset is exported as an Excel file for further analysis:

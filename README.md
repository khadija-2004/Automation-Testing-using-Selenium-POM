# Automation Testing for Daraz.pk (Selenium + Python)

## Overview
This project automates key e-commerce workflows on **Daraz.pk** using **Selenium WebDriver with Python**.  
It is designed using the **Page Object Model (POM)** architecture to keep test logic and UI locators separate.

## Technologies Used
- Python 3.x
- Selenium WebDriver
- ChromeDriver
- Page Object Model (POM)

## Project Structure
```text
DarazAutomationPOM/
│
├── drivers/
│   └── chromedriver-win64/
│       └── chromedriver.exe
│
├── pages/
│   ├── home_page.py
│   ├── search_results_page.py
│   └── product_page.py
│
├── tests/
│   └── test_daraz.py
│
├── utils/
│   └── driver_setup.py
│
└── README.md

## Implemented Features
- Project setup with Selenium and ChromeDriver
- Navigation to Daraz.pk homepage
- Product search for **"electronics"**
- Apply brand filter to refine results
- Attempt to apply price filter (500–5000)
- Count search results and validate count > 0
- Open first product from search results
- Verify free shipping availability on product page

## How to Run the Project
1. Download and extract the ZIP file from the repository.
2. Install required dependencies:
   ```bash
   pip install selenium
3. Ensure **Python 3.x** is installed.
4. Verify that the included **ChromeDriver** version matches your Chrome browser. Replace it if necessary.
5. Run the test script:
   python tests/test_daraz.py

## Design Pattern
This project uses the **Page Object Model (POM)** where:
- Each web page has its own class
- Locators and actions are separated from test logic
- Test scripts remain clean and readable

## Notes
- Filters may vary due to dynamic content on Daraz.pk
- Some filters may not apply if products or UI change
- Stable internet connection is recommended

## Author
Khadija Nafees

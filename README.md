MasQVida Reservation Automator

A Python-based automation script designed to streamline the reservation process on the MasQVida platform. This tool utilizes Selenium WebDriver to handle authentication and interact with dynamic calendar elements, ensuring efficient and repeatable booking operations.
Features

    Automated Authentication: Securely logs into the platform using configurable credentials.

    Dynamic Interaction: Uses WebDriverWait and expected_conditions to reliably handle JavaScript-rendered elements.

    Precise Targeting: Employs advanced XPath selectors to pinpoint specific time slots within the reservation grid.

    Robust Error Handling: Implements comprehensive try-except-finally blocks to manage connection timeouts, missing elements, and unexpected session interruptions, ensuring proper browser cleanup.

Prerequisites

    Python 3.x

    Google Chrome Browser

    ChromeDriver (installed automatically via webdriver-manager or present in your PATH)

    Selenium library:
    Bash

    pip install selenium


## Configuration
Edit the **CONFIGURATION** section in `main.py` before running:
```python
URL = "https://reservas.masqvida.es/paterna/login"
USER = "YOUR_EMAIL"
PASSWORD = "YOUR_PASSWORD"

Usage

Run the script directly from your terminal:
Bash

python main.py

Technical Stack

    Language: Python

    Library: Selenium WebDriver

    Selectors: XPath, By.NAME, By.PARTIAL_LINK_TEXT

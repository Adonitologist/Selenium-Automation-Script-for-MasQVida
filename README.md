# MasQVida Reservation Automator

A Python-based automation script designed to streamline the reservation process on the MasQVida platform. This tool utilizes Selenium WebDriver to handle authentication and interact with dynamic calendar elements, ensuring efficient and repeatable booking operations.

## Core Features

* **Automated Authentication:** Securely logs into the platform using external configuration files (no hardcoded credentials).
* **Dynamic Interaction:** Uses explicit `WebDriverWait` and `expected_conditions` to reliably handle JavaScript-rendered elements and prevent race conditions.
* **Precise Targeting:** Employs advanced XPath selectors to pinpoint specific time slots and locations within the reservation grid.
* **Robust Error Handling:** Implements comprehensive Object-Oriented try-except-finally blocks to manage connection timeouts, missing elements, and unexpected session interruptions while ensuring proper browser cleanup.

## Technical Stack

* **Language:** Python 3.x
* **Library:** Selenium WebDriver
* **Selectors:** XPath, CSS Selectors, By.ID

## Prerequisites

1. Python 3.8+ installed.
2. Google Chrome Browser installed.
3. Required Python libraries:
   ```bash
   pip install selenium

Configuration

The script relies on an external configuration file. Create a file named config.txt in the root directory of the script with the following format:
Plaintext

USER=your_email@example.com
PASSWORD=your_secure_password
HORAS=18:00, 19:00
FILTROS=Padel, Tenis
CUANDO=hoy

    USER / PASSWORD: Your MasQVida login credentials.

    HORAS: Comma-separated list of target class hours.

    FILTROS: Comma-separated list of keywords to filter classes.

    CUANDO: Target day (hoy, mañana, or pasado mañana).

Usage

Run the script directly from your terminal:
Bash

python main.py

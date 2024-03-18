# WL9Bet Lottery Results Scraper

The WL9Bet Lottery Results Automation System is a comprehensive Python-based solution designed to automatically scrape, process, and log lottery results from the WL9Bet website. It facilitates seamless monitoring and recording of lottery outcomes by integrating directly with Google Sheets for data storage and providing timely notifications via Telegram in case of any operational anomalies. This system is particularly beneficial for users requiring consistent updates on lottery results without manual oversight, making it an essential tool for lottery enthusiasts and analysts.

## Video Preview

[![Video Preview](https://github.com/DevRex-0201/Project-Images/blob/main/video%20preview/Py-WL9Bet-Lottery-Scraper.jpeg)](https://brand-car.s3.eu-north-1.amazonaws.com/Four+Seasons/Py-WL9Bet-Lottery-Scraper.mp4)

## Key Features

- **Automated Scraping of Lottery Results**: Utilizes web scraping techniques to extract lottery results from the WL9Bet website, ensuring accurate and up-to-date information.
- **Direct Google Sheets Integration**: Automatically updates a specified Google Sheets document with new lottery results, allowing for efficient data management and historical analysis.
- **Login Failure Notifications**: Sends notifications through Telegram in the event of unsuccessful login attempts to the WL9Bet site, enabling prompt troubleshooting.
- **Customizable Data Extraction Intervals**: Features a Tkinter GUI for setting the scraping frequency, providing flexibility in data collection based on user preferences.
- **Robust Error Handling and Retry Logic**: Implements sophisticated error handling and retry mechanisms for both web scraping and Google Sheets updates, enhancing system reliability.
- **Headless Browser Operation**: Employs a headless Chrome browser for web scraping, optimized for running on server environments without a GUI.

## System Requirements

- **Environment**: Python 3.x environment.
- **Dependencies**: `requests`, `dotenv`, `tkinter`, `selenium`, `gspread`, `oauth2client`, `bs4`, `webdriver_manager`, `asyncio`, `telegram`.
- **External Tools**: A valid Telegram bot token and chat ID for notifications, Google Sheets API credentials, and access to the Chrome web browser for Selenium WebDriver.

## Installation and Setup

### 1. Clone the Repository

Start by cloning this project to your local machine or server.

### 2. Install Required Python Libraries

Install all necessary libraries using pip:

```bash
pip install requests python-dotenv tk selenium gspread oauth2client beautifulsoup4 webdriver-manager asyncio python-telegram-bot
```

### 3. Set Up Environment Variables

Create a `.env` file in the project's root directory and define the following variable:

- `GOOGLE_SHEETS_CREDENTIALS_PATH`: The file path to your Google Sheets API credentials JSON.

### 4. Telegram Bot Configuration

Ensure you have created a Telegram bot through BotFather and obtained both the bot token and your chat ID.

### 5. Google Sheets Preparation

Share the Google Sheet intended for logging the lottery results with the email address provided in your Google Sheets API credentials file.

## Running the System

To initiate the system, execute the script via the terminal or command prompt:

```bash
python main.py
```

On launch, the script prompts for the desired scraping interval using a Tkinter dialog, then begins the automated process of extracting and logging lottery results from the WL9Bet website into the configured Google Sheet. It ensures that users have timely access to lottery results, with minimal manual intervention required.

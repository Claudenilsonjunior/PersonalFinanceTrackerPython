# Personal Finance Tracker

## Overview

The **Personal Finance Tracker** is a Python-based application that helps you manage and analyze your personal finances. It allows users to record income and expenses, categorize them, and view financial summaries over specific date ranges. The project uses a CSV file to store data and provides a simple command-line interface for interaction.

## Features

- **Add Transactions**: Record your income and expenses with details such as date, amount, category, and description.
- **View Transaction Summary**: Generate a summary of transactions over a specified date range, including total income, total expenses, and net savings.
- **Data Visualization**: Plot income and expenses over time using Matplotlib.

## Project Structure

```plaintext
Personal Finance Tracker/
│
├── main.py                # Main script to run the application
├── data_entry.py          # Script to handle data input and validation
├── finance.csv            # CSV file where financial data is stored
├── requirements.txt       # List of dependencies
└── venv/                  # Virtual environment (not included in the repository)
```
# Detailed Explanation of the Code
## *'main.py'*

* CSV Class:
  * Handles operations related to the CSV file (finance.csv), including initialization, adding new entries, and filtering transactions by date range.
  * initialize_csv: Checks if the CSV file exists; if not, it creates one with the necessary columns.
  * add_entry: Appends a new transaction to the CSV file.
  * get_transactions: Filters transactions between specified start and end dates, and provides a summary of income, expenses, and net savings.
 
* add Function:
  * Prompts the user to input details for a new transaction and saves it using the CSV.add_entry method.

* plot_transactions Function:
  * Visualizes the income and expenses over time using Matplotlib.

* main Function:
  * Serves as the entry point for the application, providing a simple CLI to add transactions, view summaries, and plot data.

# *data_entry.py*

*  **Input Handling Functions:**
    *  **get_date:** Validates and formats date input.
    * **get_amount:** Validates and ensures the entered amount is positive.
    * **get_category:** Ensures the category is "Income" or "Expense."
    * **get_description:** Allows optional input for transaction descriptions.

# Example Usage

1. **Running the Application:**

  * Start the application by running main.py:

```bash
python main.py
```

  * You can add a transaction, view transactions, or exit the application.

2. **Adding a Transaction:**

  * Select "1" to add a transaction.
  * Enter the date, amount, category (Income or Expense), and an optional description.
  * The transaction will be recorded in finance.csv.

3. **Viewing Transactions and Summary:**

  *  Select "2" to view transactions within a specific date range.
  *  Enter the start and end dates, and the application will display the transactions, along with a summary of total income, total expenses, and net savings.

4. **Plotting Transactions:**

  * After viewing transactions, you can choose to plot the data.
  * A graph showing income and expenses over time will be displayed.

# Setup Instructions

## *1. Clone the Repository*

First, clone the repository from GitHub:

```bash
git clone https://github.com/Claudenilsonjunior/PersonalFinanceTrackerPython.git
cd personal-finance-tracker
```

## *2. Set Up the Virtual Environment*

Create and activate a virtual environment:

```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

## *3. Install Dependencies*

Install the necessary Python libraries listed in requirements.txt:

```bash
pip install -r requirements.txt
```

## *4. Running the Application*

To start the application, run the main.py script:

```bash
python main.py
```

# Dependencies

The project relies on the following Python libraries:

* pandas: For data manipulation and analysis.
* matplotlib: For plotting income and expenses.
* csv: For handling CSV file operations.

These dependencies are listed in the requirements.txt file and can be installed using 
```bash
pip install -r requirements.txt.
```
# Contributing

If you want to contribute to this project, feel free to fork the repository and submit a pull request. Contributions, whether it’s bug fixes, improvements, or new features, are welcome!

# Contact

For any questions or feedback, please contact <claudenilsonjunior2@gmail.com>

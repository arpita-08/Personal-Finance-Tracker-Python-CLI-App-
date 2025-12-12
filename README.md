#Personal Finance Tracker (Python CLI App)

A simple and efficient command-line Personal Finance Tracker built using Python.
This tool allows users to record income and expenses, view transaction summaries within a date range, and generate visual plots for financial insights.

Features
1. Add Transactions
Record:
Date
Amount
Category (Income or Expense)
Description
Entries are appended directly to finance_data.csv.

2. View Transactions by Date Range
Fetch and display all transactions between two dates:
Filter results using Pandas
Shows a neat table in the console
Calculates:
Total Income
Total Expense
Net Savings

3. Visualize Financial Data
Generate a Matplotlib line chart showing:
Daily Income
Daily Expense
A clean time-series plot helps you quickly spot trends.
Project Structure
│
├── main.py              # Main application loop
├── data_entry.py        # Input validation + data collection functions
├── finance_data.csv     # Stores all financial transactions
└── README.md            # Documentation

How It Works
CSV Handling
The CSV class handles:
Creating the file if it doesn't exist
Appending new entries
Filtering transactions using a date range
Summarizing income vs expenses

User Interaction
All user inputs (date, amount, category, description) are validated using helper functions in data_entry.py.

Date Format
All dates follow:
dd-mm-yyyy

Requirements
Before running:
pip install pandas matplotlib
Python version: 3.8+ recommended.

How to Run
Open your terminal and execute:
python main.py
Then choose between:
Add a new transaction
View transactions and summary
Exit
If you choose option 2, you'll also be offered a graph preview.

Sample CSV Data
The project includes sample financial data in:
finance_data.csv
This helps you test analysis and plotting features immediately.

Future Improvements (Scope in this Project)
Category-wise analysis
Monthly reports
Export to PDF
GUI interface
Budget alerts

# Personal Finance Tracker

Welcome to the Personal Finance Tracker! This project is designed to help you keep track of your income and expenses over time. Using Python, pandas, and Matplotlib, this tool allows you to easily manage your finances and visualize your financial transactions.

## Features

- **Add Transactions:** Easily add new income or expense transactions with date, amount, category, and description.
- **View Transactions:** Filter and view transactions within a specified date range.
- **Summary:** Get a summary of total income, total expenses, and net savings within the chosen date range.
- **Plot Transactions:** Visualize income and expenses over time with a plot.

## Requirements

- Python 3.6+
- pandas
- matplotlib

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/personal-finance-tracker.git
   cd personal-finance-tracker
   ```

2. Install the required Python packages:
   ```sh
   pip install pandas matplotlib
   ```

## Usage

Run the main script to start using the Personal Finance Tracker:
```sh
python main.py
```

### Adding a New Transaction

1. Select option `1` from the main menu to add a new transaction.
2. Follow the prompts to enter the date, amount, category (Income or Expense), and description (optional).

### Viewing Transactions and Summary

1. Select option `2` from the main menu to view transactions within a specific date range.
2. Enter the start date and end date in `dd-mm-yyyy` format.
3. The transactions within the specified date range will be displayed along with a summary of total income, total expenses, and net savings.
4. You can choose to view a plot of the transactions by entering `y` when prompted.

### Exiting the Program

Select option `3` from the main menu to exit the program.

## Data Entry Functions

The following helper functions are used for data entry:
- `get_date(prompt, allow_default=False)`: Prompts the user to enter a date and validates the input.
- `get_amount()`: Prompts the user to enter the amount and validates the input.
- `get_category()`: Prompts the user to enter the category (`I` for Income, `E` for Expense) and validates the input.
- `get_description()`: Prompts the user to enter a description (optional).

## Data Storage

Transactions are stored in a CSV file named `finance_data.csv` with the following columns:
- `date`: The date of the transaction in `dd-mm-yyyy` format.
- `amount`: The amount of the transaction.
- `category`: The category of the transaction (`Income` or `Expense`).
- `description`: A brief description of the transaction.

## Plotting Transactions

The `plot_transactions(df)` function is used to generate a plot of income and expenses over time. The function uses the pandas library to resample the data by day and Matplotlib to create the plot.

## Example CSV Data

Here is an example of the `finance_data.csv` file:
```csv
date,amount,category,description
01-07-2024,1000,Income,Salary
02-07-2024,50,Expense,Groceries
03-07-2024,150,Expense,Utilities
04-07-2024,200,Income,Freelance Work
05-07-2024,75,Expense,Restaurant
06-07-2024,100,Expense,Transport
07-07-2024,500,Income,Bonus
08-07-2024,30,Expense,Snacks
09-07-2024,250,Income,Stock Dividends
10-07-2024,90,Expense,Entertainment
11-07-2024,60,Expense,Coffee
12-07-2024,120,Expense,Gas
13-07-2024,80,Expense,Books
14-07-2024,150,Expense,Clothing
15-07-2024,1100,Income,Salary
16-07-2024,40,Expense,Stationery
17-07-2024,180,Expense,Utilities
18-07-2024,250,Income,Freelance Work
19-07-2024,70,Expense,Restaurant
20-07-2024,130,Expense,Transport
21-07-2024,600,Income,Bonus
22-07-2024,35,Expense,Snacks
23-07-2024,300,Income,Stock Dividends
24-07-2024,100,Expense,Entertainment
25-07-2024,55,Expense,Coffee
26-07-2024,140,Expense,Gas
27-07-2024,90,Expense,Books
28-07-2024,170,Expense,Clothing
29-07-2024,1200,Income,Salary
30-07-2024,45,Expense,Stationery
31-07-2024,190,Expense,Utilities
20-07-2023,124.0,Expense,Groceries
```

## License

This project is licensed under the MIT License.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

---

Thank you for using the Personal Finance Tracker! If you have any questions or suggestions, feel free to open an issue on GitHub.

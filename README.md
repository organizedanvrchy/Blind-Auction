# Blind Auction (Silent Auction) (CLI)

## Summary
This Python script simulates a silent auction where participants can enter their names and bids. The program collects all bids and determines the highest bidder as the winner. The program supports multiple bidders and clears the console screen after each bid to maintain privacy. Once all bids are entered, the program announces the winner with the highest bid.

## Features
- **Bid Collection**: The program uses a dictionary (`auction_dict`) to store bidder names as keys and their corresponding bids as values.
- **Input Validation**: The program ensures that bids are valid numbers by using a `try-except` block to handle invalid inputs (e.g., non-numeric values).
- **Console Clearing**: The program clears the console screen after each bid to maintain privacy and provide a clean interface for the next bidder. This is done using `os.system("cls")` for Windows or `os.system("clear")` for Unix-based systems.
- **Winner Determination**: The program uses the `max()` function with a custom key (`auction_dict.get`) to determine the highest bidder.
- **User Interaction**: The program prompts users to enter their names and bids, and asks if there are additional bidders after each entry.
- **ASCII Art**: The `logo` module is used to display a logo or visual element at the start of the program, enhancing the user experience.
- **Loop Control**: A `while` loop is used to continuously collect bids until there are no more bidders.

## How to Use
1. Run the script in a Python environment.
2. Enter your name and bid when prompted.
3. If there are additional bidders, the console will clear, and the next bidder can enter their information.
4. Once all bids are entered, the program will announce the winner with the highest bid.

## Requirements
- Python 3.x
- The `logo` module (for displaying the auction logo).

## Running the Program
To run the program, simply execute the script in your Python environment:
```bash
python main.py
```

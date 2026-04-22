💰 Tip Calculator

A simple Python program that calculates how much each person should pay when splitting a bill, including tip.

🚀 Features
Takes total bill amount as input
Allows user to choose tip percentage (10%, 12%, or 15%)
Splits the bill among multiple people
Rounds the final amount to 2 decimal places
🧠 How It Works
User enters the total bill amount
User selects a tip percentage
User enters number of people sharing the bill
Program calculates:
Tip amount
Total bill including tip
Amount per person
🧾 Example
Welcome to the tip calculator!
What was the total bill?
$100
How much tip would you like to give? 10, 12, or 15
10
How many people to split the bill?
2
Each person should pay $55.0.
🛠️ Code
print("Welcome to the tip calculator!")

bill = float(input("What was the total bill?\n$"))
tip = int(input("How much tip would you like to give? 10, 12, or 15\n"))
people = int(input("How many people to split the bill?\n"))

tip_as_percent = tip / 100
total_tip_amount = bill * tip_as_percent
total_bill = bill + total_tip_amount
bill_per_person = total_bill / people
final_amount = round(bill_per_person, 2)

print(f"Each person should pay ${final_amount}.")
⚠️ Notes
Make sure to enter valid numbers
Tip percentage should be one of: 10, 12, or 15
The result is rounded to 2 decimal places for currency formatting
📌 Future Improvements
Input validation (handle invalid inputs)
Support for custom tip percentages
Currency formatting (e.g., always show 2 decimal places like $55.00)

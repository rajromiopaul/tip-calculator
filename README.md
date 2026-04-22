# 💰 Tip Calculator

A simple Python program that helps split a bill among multiple people, including a tip.

---

## 📌 Features

- Takes total bill amount as input
- Allows user to choose tip percentage (10%, 12%, 15%)
- Splits the total bill evenly among a group
- Rounds the final amount to 2 decimal places

---

## 🧠 How It Works

1. User enters the total bill amount
2. User selects a tip percentage
3. User enters number of people
4. Program calculates:
   - Tip amount
   - Total bill (including tip)
   - Amount each person should pay

---

## 🧾 Example


Welcome to the tip calculator!
What was the total bill?
$100
How much tip would you like to give? 10, 12, or 15
10
How many people to split the bill?
4
Each person should pay $27.5.


---

## 🛠️ Code

```python
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
```
🚀 How to Run
Make sure Python is installed
Save the file as tip_calculator.py
Run the program:
python tip_calculator.py
⚠️ Note
Ensure valid numeric inputs
Tip percentages should be one of: 10, 12, or 15

# cwon150-PythonCoding_Project2_Tip-Calculator-uses_in_USA

# If the bill was $150.00, split between 5 people, with 12% tip.  Each person should pay (150.00 / 5) * 1.12 = 33.6  Format the result to 2 decimal places = 33.60  Thus everyone's share of the total bill is $30.00 plus a $3.60 tip.

# Example Input

Welcome to the tip calculator!

What was the total bill? $150

How much tip would you like to give? 10, 12, or 15? 12

How many people to split the bill? 5

Each person should pay: $33.60

# Python coding starts at the following below:

print("Welcome to the tip calculator!")

total_bill = float(input("What was the total bill? $"))

tip_percent = float(input("How much tip would you like to give? 10, 12, or 15? "))

tip_percent2 = tip_percent/100 + 1

split_num = float(input("How many people to split the bill? "))

result = (total_bill / split_num) * tip_percent2

print(f"Each person should pay: ${result:.2f}")

# Alternatively, you can code as following below:

print("Welcome to the tip calculator!")

total_bill = float(input("What was the total bill? $"))

tip = int(input("How much tip would you like to give? 10, 12, or 15? "))

split_num = int(input("How many people to split the bill? "))

bill_with_tip = tip / 100 * total_bill + total_bill

result = bill_with_tip / split_num

# The reason that I do not add -  final_result = round(result,2) and then I code - print(final_result) at the end because it is a formating problem. We will only get the result of $33.6 [(150/5)*1.12 = 33.6]. 

print(f"Each person should pay: ${result:.2f}")





# Python-3
# Problem 3: CD Interest

# Get user input for CD principle and years to maturity
principle = float(input("Enter CD principle amount: $"))
years_to_maturity = int(input("Enter years to maturity: "))

# Determine interest rate based on the schedule
if principle > 100000:
    interest_rate = 0.06
elif 50000 <= principle <= 100000 and years_to_maturity == 10:
    interest_rate = 0.05
elif 50000 <= principle <= 100000 and years_to_maturity == 5:
    interest_rate = 0.04
else:
    interest_rate = 0.02

# Calculate first year interest
interest_amount = principle * interest_rate

# Display results
print(f"\nPrinciple: ${principle:.2f}")
print(f"Interest Rate: {interest_rate * 100:.2f}%")
print(f"Interest Amount for First Year: ${interest_amount:.2f}")

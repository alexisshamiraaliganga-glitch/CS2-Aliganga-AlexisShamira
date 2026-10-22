RATE = 12.90

# Validate student name:
while True:
    name = input("Enter customer name: ")
    
    if name.strip() != "":
        break
    else:
        print("Invalid name. Cannot be empty. Please try again")
        
# Validate Previous reading
while True:
    previous = float(input("Enter previous meter reading: "))
    
    if previous and 0 <= float(previous):
        previous = float(previous)
        break
    else:
        print("Invalid Previous Meter reading. Enter a number greater than or equal to 0")
        
# Validate Current reading
while True:
    current = float(input("Enter current meter reading: "))
    
    if current and previous <= float(current):
        current = float(current)
        break
    else:
        print("Invalid Current Meter reading. Must be greater than the Previous Meter Reading. Try again")
        
consumption = current - previous
total_bill = consumption * RATE

print("\nCustomer:", name)
print("Electricity Consumption:", consumption, "kWh")
print("Total Bill: PHP", round(total_bill, 2))

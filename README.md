# Budget-Baby-
“Budget Baby” will display a budgeting tool. This budgeting tool will be beneficial to anyone serious about their finances. My program will insist in expenses, revenue, and your designated budgeted balance. It will add up all of your input totals and generate your proper budget balance. 



#Main Module
expense = 0.0
budget = 0.0
difference = 0.0
expenseTotal = 0.0

total_expense = 0
keep_going = 'y'


#Input Module
budget = float(input("What is your budget for the month?"))
print("Please begin entering the amounts of each of your monthly expenses:")

while keep_going == 'y':
    expense = float(input("Monthly expense amount? $"))
#*Having an issue keeping the expense running total at the end of the program?*
    total_expense = total_expense + expense
    keep_going = input("Do you have any other expenses? (Enter y for yes.)")

#Calculations Module
if expense < budget:
    difference = budget - expense
    print("You were $", difference, " under budget.")

elif expense > budget:
    difference = expense - budget
    print("You were $", difference, " over budget.")

else:
    print("You were right on budget. Great Job!!!")


input("Press enter to exit.")

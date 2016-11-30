# Problem Statement
Create a simple tip calculator. The program should prompt
for a bill amount and a tip rate. The program must compute
the tip and then display both the tip and the total amount of
the bill.

*Nouns
    bill amont
    tip rate
    tip
    total amount

*Verbs
    prompt
    compute
    display


*Example output
    What is the bill? $200
    What is the tip percentage? 15
    The tip is $30.00
    The total is $230.00

# Discover Input, Processes, and Output
Inputs:
    bill amount
    tip rate
Processes:
    calculate  the tip
Outputs:
    tip amount
    total amount

#Driving Design with Tests (TDD)
Input:
    bill amount: 11.25
    tip rate: 15
Expected result:
    Tip: $1.50
    Total: $11.50

Input:
bill amount: 11.25
tip rate: 15
Expected result:
Tip: $1.69
Total: $12.94
    Actual results"
#Writing the Algorithm in Pseudocode
TipCalculator
    Initialize billAmount to 0
    Initialize tip to 0
    Initialize tipRate to 0
    Initialize total to 0
    Prompt for billAmount with "What is the bill amount?"
    Prompt for tipRate with "What is the tip rate?"
    convert billAmount to a number
    convert tipRate to a number
    tip = billAmount * (tipRate / 100)
    round tip up to nearest cent
    total = billAmount + tip
    Display "Tip: $" + tip
    Display "Total: $" + total
End

# Writing the Code
       ##Constraints
      - Enter the tip as a percentage. For example, a 15% tip
       would be entered as 15, not 0.15. Your program should
       handle the division.
      - Round fractions of a cent up to the next cent.]

#Challenges
    -Ensure that the user can enter only numbers for the bill
    amount and the tip rate. If the user enters non-numeric
    Chapter 1. Turning Problems into Code • 8
    More books at 1Bookcase.com report erratum • discuss
    values, display an appropriate message and exit the
    program. Here’s a test plan as an example:

    Input:
    bill amount: abcd
    tip rate: 15
    Expected result: Please enter a valid number for
    the bill amount.
    -Instead of displaying an error message and exiting the
     program, keep asking the user for correct input until it
     is provided.
    -Don’t allow the user to enter a negative number.
    -Break the program into functions that do the computations.
    -• Implement this program as a GUI program that automatically
     updates the values when any value changes.
     -Instead of the user entering the value of the tip as a
      percentage, have the user drag a slider that rates satisfaction
      with the server, using a range between 5% and
      20%.

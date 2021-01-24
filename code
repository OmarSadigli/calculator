from replit import clear
from art import logo
#Calculator

def add(n1, n2):
  return n1 + n2

def subtract(n1, n2):
  return n1 - n2

def multiply(n1, n2):
  return n1 * n2

def divide(n1, n2):
  return n1 / n2

operations = {
  "+": add,
  "-": subtract,
  "*": multiply,
  "/": divide,
}

def calculator():
  print(logo)
  num1 = float(input("What's the first number?: "))
  for operator in operations:
    print(operator)
    
  should_continue = True

  while should_continue:
    operator_choice = input("Pick an operation: ")
    num2 = float(input("What's the next number?: "))
    calculation_function = operations[operator_choice]
    answer = calculation_function(num1, num2)

    print(f"{num1} {operator_choice} {num2} = {answer}")

    ask_user = input(f"Type 'y' to continue calculating with {answer}, or type 'n' to exit.: ")

    if ask_user == 'y':
      num1 = answer
    else:
      clear()
      calculator()

calculator()   

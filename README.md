# Simple Python Calculator

A lightweight calculator built with Python, supporting basic arithmetic operations (addition, subtraction, multiplication, division) with a command-line interface. Ideal for beginners learning Python fundamentals.

## Features
- ➕➖✖️➗ Basic operations (+, -, *, /)
- 🖥️ Command-line interface (CLI)
- ❌ Error handling (e.g., division by zero, invalid inputs)
- 🔄 Continuous calculations until user exits

## Installation
1. Ensure Python 3.x is installed:
   ```bash
   python --version
Clone the repository:

bash
git clone https://github.com/RadiantCOREX64/simple-python-calculator.git
Run the calculator:

bash
cd simple-python-calculator
python calculator.py
Usage
Run the script and follow the prompts:

plaintext
Enter first number: 5
Enter operation (+, -, *, /): *
Enter second number: 3
Result: 15.0
Code Structure
python
# calculator.py
def main():
    while True:
        try:
            num1 = float(input("Enter first number: "))
            op = input("Enter operation (+, -, *, /): ")
            num2 = float(input("Enter second number: "))
            
            if op == "+":
                print(f"Result: {num1 + num2}")
            elif op == "-":
                print(f"Result: {num1 - num2}")
            elif op == "*":
                print(f"Result: {num1 * num2}")
            elif op == "/":
                print(f"Result: {num1 / num2}")
            else:
                print("Invalid operation!")
        except ValueError:
            print("Invalid input! Please enter numbers.")
        except ZeroDivisionError:
            print("Error: Division by zero!")
        
        if input("Continue? (y/n): ").lower() != 'y':
            break

if __name__ == "__main__":
    main()
Future Enhancements
Add GUI (Tkinter/PyQt)

Support scientific operations (e.g., exponents, square roots)

Package as a PIP-installable tool

Contributing
Pull requests welcome! For major changes, open an issue first.

License
MIT


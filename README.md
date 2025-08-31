🧮 Simple Calculator in C

A simple, interactive, and user-friendly calculator built in C. Perform basic arithmetic operations like addition, subtraction, multiplication, and division right from your terminal. 🚀

Features ✨

Addition, Subtraction, Multiplication, Division

Handles division by zero gracefully ❌➗

Interactive menu for easy navigation

Supports continuous calculations until the user decides to exit 🔄

Cross-platform screen clearing (Windows & Linux/Mac) 🖥️

Clean and readable output with formatted results

Screenshots 📸
=== Simple Calculator ===
Welcome to the Calculator!

Available Operations:
1. Addition (+)
2. Subtraction (-)
3. Multiplication (*)
4. Division (/)
5. Exit
------------------------
Enter your choice (1-5): 1
Enter first number: 25
Enter second number: 10

Result: 25.00 + 10.00 = 35.00

Do you want to perform another calculation? (y/n): y

Installation 💻

Clone the repository

git clone https://github.com/yourusername/simple-calculator-c.git
cd simple-calculator-c


Compile the program

gcc calculator.c -o calculator


Run the calculator

./calculator      # Linux/Mac
calculator.exe    # Windows

Usage 🖱️

Launch the program.

Choose an operation from the menu (1–5).

Enter two numbers.

See the result displayed in a neat and readable format.

Choose whether to perform another calculation or exit.

Code Structure 🏗️

main() – Handles user input and program flow

displayMenu() – Shows the list of available operations

add(), subtract(), multiply(), divide() – Arithmetic functions

clearScreen() – Clears terminal screen based on OS

Future Improvements 🚀

Add advanced operations like modulus, power, and square root

Implement history of calculations

Create a graphical version using C GUI libraries

Add keyboard shortcuts for faster input

Author ✍️

Ram Khandekar

Student & C Programmer

Portfolio: https://astas-portfolio.netlify.app

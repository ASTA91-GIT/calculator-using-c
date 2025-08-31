# C Programming Calculator

A comprehensive console-based calculator application written in C programming language. This project demonstrates fundamental C programming concepts including functions, control structures, error handling, and user input processing.

## 🧮 Calculator Overview

The C Calculator provides a menu-driven interface for performing basic arithmetic operations (addition, subtraction, multiplication, division) with robust error handling and a user-friendly experience.

## ✨ Features

- **Four Basic Operations**: Addition, subtraction, multiplication, and division
- **Menu-Driven Interface**: Clear, numbered menu for easy navigation
- **Error Handling**: Division by zero protection and input validation
- **Continuous Operation**: Option to perform multiple calculations
- **Cross-Platform**: Works on Windows, Linux, and macOS
- **User-Friendly**: Clear prompts and formatted output
- **Modular Design**: Well-organized functions for each operation

## 🛠️ Technologies Used

- **C Programming Language**: Core implementation
- **Standard C Library**: `stdio.h`, `stdlib.h`
- **Functions**: Modular programming approach
- **Control Structures**: `switch-case`, `if-else`, `while` loops
- **Input/Output**: `printf()`, `scanf()` functions
- **Error Handling**: Conditional checks and validation

## 🚀 How to Compile and Run

### Prerequisites
- C compiler (GCC recommended) installed on your system
- Basic understanding of command line/terminal

### Compilation & Execution

#### On Windows:
```bash
# Navigate to project directory
cd PROJECTS/FRONT_END/projects

# Compile the program
gcc c_simple_calculator.c -o calculator.exe

# Run the program
calculator.exe
```

#### On Linux/macOS:
```bash
# Navigate to project directory
cd PROJECTS/FRONT_END/projects

# Compile the program
gcc c_simple_calculator.c -o calculator

# Run the program
./calculator
```

## 🎯 How to Use

1. **Start the Program**: Compile and run the executable
2. **View Menu**: The program displays available operations
3. **Select Operation**: Enter a number (1-5) to choose an operation
4. **Enter Numbers**: Provide two numbers for the calculation
5. **View Result**: See the formatted result of your calculation
6. **Continue or Exit**: Choose to perform another calculation or exit

## 📋 Code Structure

### Main Functions

#### `main()`
- Program entry point
- Handles the main program loop
- Manages user interaction and menu flow
- Coordinates all calculator operations

#### `displayMenu()`
- Prints the operation menu
- Shows available calculator functions
- Provides clear user guidance

#### Arithmetic Functions
- `add(float a, float b)`: Performs addition
- `subtract(float a, float b)`: Performs subtraction
- `multiply(float a, float b)`: Performs multiplication
- `divide(float a, float b)`: Performs division with error checking

#### `clearScreen()`
- Cross-platform screen clearing
- Uses conditional compilation for different operating systems

### Key Features Explained

#### Menu System
```c
void displayMenu() {
    printf("Available Operations:\n");
    printf("1. Addition (+)\n");
    printf("2. Subtraction (-)\n");
    printf("3. Multiplication (*)\n");
    printf("4. Division (/)\n");
    printf("5. Exit\n");
    printf("------------------------\n");
}
```
- Clear, numbered menu for easy navigation
- Consistent formatting and user guidance

#### Error Handling
```c
case 4:
    if (num2 == 0) {
        printf("Error: Division by zero is not allowed!\n\n");
        continue;
    }
    result = divide(num1, num2);
    operator = '/';
    break;
```
- Prevents division by zero errors
- Provides clear error messages
- Allows program to continue safely

#### Input Validation
```c
if (choice < 1 || choice > 5) {
    printf("Invalid choice! Please enter a number between 1 and 5.\n\n");
    continue;
}
```
- Validates user input range
- Prevents invalid menu selections
- Maintains program stability

## 🎨 User Interface Features

- **Clear Menu**: Numbered options for easy selection
- **Formatted Output**: Professional-looking results display
- **Error Messages**: Helpful feedback for invalid inputs
- **Progress Indicators**: Shows current operation being performed
- **Exit Option**: Clean way to terminate the program

## 🔧 Customization Options

### Easy Modifications

#### Add New Operations
```c
// Add to displayMenu() function
printf("6. Power (^)\n");
printf("7. Square Root (√)\n");

// Add to main() switch statement
case 6:
    result = power(num1, num2);
    operator = '^';
    break;
case 7:
    result = sqrt(num1);
    operator = '√';
    break;
```

#### Change Number Precision
```c
// Modify the result display format
printf("\nResult: %.3f %c %.3f = %.3f\n\n", num1, operator, num2, result);
// Change .2f to .3f for 3 decimal places
```

#### Add Memory Functions
```c
// Add memory storage variables
float memory = 0.0;

// Add memory operations
case 8:
    memory = result;
    printf("Result stored in memory: %.2f\n", memory);
    break;
case 9:
    num1 = memory;
    printf("Memory value loaded: %.2f\n", memory);
    break;
```

## 🧪 Testing the Calculator

### Test Cases to Try

#### Basic Operations
1. **Addition**: 5 + 3 = 8
2. **Subtraction**: 10 - 4 = 6
3. **Multiplication**: 6 × 7 = 42
4. **Division**: 15 ÷ 3 = 5

#### Edge Cases
1. **Division by Zero**: 10 ÷ 0 (should show error)
2. **Large Numbers**: 999999 + 1
3. **Decimal Numbers**: 3.14 + 2.86
4. **Negative Numbers**: -5 + 3

#### Input Validation
1. **Invalid Menu Choice**: Enter 6 or 0
2. **Non-numeric Input**: Enter letters instead of numbers
3. **Boundary Values**: Very large or very small numbers

### Sample Session
```
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
Enter first number: 15.5
Enter second number: 7.3

Result: 15.50 + 7.30 = 22.80

Do you want to perform another calculation? (y/n): y

Available Operations:
1. Addition (+)
2. Subtraction (-)
3. Multiplication (*)
4. Division (/)
5. Exit
------------------------
Enter your choice (1-5): 4
Enter first number: 20
Enter second number: 0
Error: Division by zero is not allowed!

Available Operations:
1. Addition (+)
2. Subtraction (-)
3. Multiplication (*)
4. Division (/)
5. Exit
------------------------
Enter your choice (1-5): 5
Thank you for using the calculator!
```

## 📚 Learning Objectives

This project helps you learn:
- **C Programming Basics**: Variables, data types, operators
- **Functions**: Defining, declaring, and calling functions
- **Control Structures**: Switch statements, if-else, loops
- **Input/Output**: printf() and scanf() functions
- **Error Handling**: Input validation and error checking
- **Modular Programming**: Organizing code into functions
- **Cross-Platform Development**: Conditional compilation
- **User Interface Design**: Creating intuitive menus

## 🔗 Related Links

- **GitHub Repository**: [View Code](https://github.com/ASTA91-GIT/portfolio/blob/main/projects/c_simple_calculator.c)
- **All Projects**: [Portfolio Projects](https://github.com/ASTA91-GIT/portfolio/tree/main/projects)
- **Main Portfolio**: [ASTA Portfolio](https://asta91-git.github.io/portfolio)

## 🤝 Contributing

Feel free to:
- Add new mathematical operations (power, square root, etc.)
- Implement memory functions (store, recall, clear)
- Add scientific calculator features
- Improve error handling and validation
- Create a graphical user interface version
- Add unit conversion features

## 📄 License

This project is part of the ASTA Portfolio and is available under the MIT License.

---

**Happy Calculating! 🧮**

*This project demonstrates fundamental C programming concepts while providing a practical calculator application.*

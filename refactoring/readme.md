# Factorial Calculation Script

This repository contains a simple Python script, `factorial.py`, which calculates the factorial of a given number. The purpose of this example is to showcase the functionality of GitHub Copilot in assisting developers with **refactoring Python code into Go**. By using this script as a base, we can demonstrate how Copilot’s suggestions can be leveraged to convert Python code into idiomatic Go code.

---

## Project Overview

### About the Script
The `factorial.py` script defines a `factorial` function to calculate the factorial of a non-negative integer. This calculation is a basic but powerful example, as it includes fundamental programming concepts such as:
- Conditional statements
- Looping structures
- Error handling
- Function definitions

### Why This Script?
This script is a great candidate for refactoring because:
1. **Simplicity**: It is easy to understand and compact, making it suitable for conversion without overwhelming complexity.
2. **Common Logic**: Factorial calculations are familiar in both Python and Go, allowing us to focus on language-specific syntax and idioms.
3. **Demonstrative Value**: The script showcases core programming constructs (e.g., loops, conditionals) that will allow us to explore how Copilot translates these from Python to Go.

---

## Example Script: `factorial.py`

Below is the Python code contained in `factorial.py`:

```python
def factorial(n):
    """Calculate the factorial of a number."""
    if n < 0:
        return "Factorial not defined for negative numbers."
    elif n == 0 or n == 1:
        return 1
    else:
        result = 1
        for i in range(2, n + 1):
            result *= i
        return result

# Example usage
if __name__ == "__main__":
    num = 5
    print(f"The factorial of {num} is {factorial(num)}")

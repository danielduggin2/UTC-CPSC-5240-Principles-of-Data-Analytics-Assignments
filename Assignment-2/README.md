```markdown
# 📌 Assignment 2 - Fibonacci Sequence Calculator

### 👤 Author: Daniel Duggin  
### 📖 Course: CPSC 5240  

---

## 📜 Overview  
This program calculates the **nth Fibonacci number** based on user input. It includes:
- A function `fibonacci(n)` that handles:
  - **Edge cases** where `n ≤ 0` (invalid input).
  - **Base cases** where `n = 1 or 2`, returning `1`.
  - **Iterative approach** for `n > 2`, updating values step by step.
- A **main program** that:
  - Prompts the user for input.
  - Calls the Fibonacci function.
  - Prints the result while handling invalid inputs gracefully.

---

## 📥 Importing Libraries  
```python
# No external libraries are needed for basic Fibonacci calculation,
# but you may import these if extending functionality.
import sys
import time
```

---

## 🔢 Fibonacci Function Implementation  
```python
def fibonacci(n):
    """Returns the nth Fibonacci number using an iterative approach."""
    if n <= 0:
        return "Invalid input. Please enter a positive integer."
    elif n == 1 or n == 2:
        return 1
    
    a, b = 1, 1
    for _ in range(3, n + 1):
        a, b = b, a + b
    return b
```

### 🔹 Explanation  
- If `n ≤ 0`, the function returns an **error message**.
- If `n = 1 or 2`, the function returns `1` (base cases).
- If `n > 2`, it starts with:
  - `a = 1`, `b = 1` (Fibonacci sequence base values).
  - Iterates from `3` to `n`, updating `a` and `b` at each step.
- Returns `b` as the **nth Fibonacci number**.

---

## 🎯 Main Program Execution  
```python
def main():
    try:
        n = int(input("Enter a positive integer: "))
        result = fibonacci(n)
        print(f"The {n}th Fibonacci number is: {result}")
    except ValueError:
        print("Invalid input. Please enter an integer.")
        
if __name__ == "__main__":
    main()
```

### 🔹 Explanation  
- **Asks for user input** (`n`).
- **Handles non-integer input** using `try-except` for errors.
- Calls `fibonacci(n)` and prints the result.

---

## 🏁 Example Output  
```
Enter a positive integer: 7
The 7th Fibonacci number is: 13
```

```
Enter a positive integer: -2
Invalid input. Please enter a positive integer.
```

```
Enter a positive integer: five
Invalid input. Please enter an integer.
```

---

## 🔧 Possible Enhancements  
✅ Optimize using **memoization** or **dynamic programming**.  
✅ Implement a **recursive** version of the Fibonacci function.  
✅ Extend the program to **calculate Fibonacci series up to nth number**.  

---

## 🗂️ File Structure  
```
Assignment-2/
│── fibonacci.py  # Python script containing the Fibonacci function
│── README.md     # Explanation of the code
```

---

### 🚀 Notes  
- This approach **efficiently calculates Fibonacci numbers** iteratively.  
- **Avoids recursion stack overflow** for large values of `n`.  

📌 **Next Steps:** Explore different Fibonacci sequence implementations!  

---
```

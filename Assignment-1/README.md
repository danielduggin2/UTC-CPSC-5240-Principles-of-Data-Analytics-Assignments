```markdown
# Assignment 1

## 📌 Importing Libraries

```python
import sklearn
import numpy as np
import pandas as pd
import matplotlib
import scipy
import seaborn
```

### 🔹 Explanation
In this portion of the code, we import the following libraries:

- **Scikit-learn (`sklearn`)** - Machine learning library
- **NumPy (`np`)** - Numerical computing
- **Pandas (`pd`)** - Data manipulation and analysis
- **Matplotlib (`matplotlib`)** - Data visualization
- **SciPy (`scipy`)** - Scientific computing
- **Seaborn (`seaborn`)** - Statistical data visualization

We don’t have to, but we can **abbreviate** certain libraries for convenience (e.g., `pandas` as `pd` or `numpy` as `np`). However, using shorthand names sometimes causes issues when retrieving the version of a library.

---

## 🏗️ Defining the Main Function

```python
def main():
    print("Hello, I am Daniel Duggin")
    print("scikit-learn version:", sklearn.__version__)
    print("numpy version:", np.__version__)
    print("pandas version:", pd.__version__)
    print("matplotlib version:", matplotlib.__version__)
    print("scipy version:", scipy.__version__)
    print("seaborn version:", seaborn.__version__)
```

### 🔹 Explanation
- We define a function using the **`def` keyword**.
- The function **prints**:
  - A greeting
  - The version numbers of the imported libraries
- **`library.__version__`** retrieves the installed version of a package.
- The **double underscores (`__version__`)** indicate that it is a **special attribute** in Python.

---

## 🏁 Running the Script

```python
if __name__ == "__main__":
    main()
```

### 🔹 Explanation
- This `if` statement ensures that `main()` **only runs when the script is executed directly**.
- If the script is **imported** as a module in another script, `__name__` will not be `"__main__"`, and `main()` won’t execute.
- This is useful when we want to use the functions in other Python files.

---

## 📌 Summary
✅ Imported essential libraries  
✅ Created a `main()` function to print information  
✅ Used `if __name__ == "__main__"` to ensure the script runs properly  

---

### 🎯 Example Output
```
Hello, I am Daniel Duggin
scikit-learn version: 1.2.2
numpy version: 1.26.4
pandas version: 2.1.1
matplotlib version: 3.7.2
scipy version: 1.11.3
seaborn version: 0.12.2
```

---

### 📌 Next Steps
1. **Modify the script** to perform additional computations.
2. **Experiment with different libraries** and explore their functions.
3. **Use virtual environments** to manage library versions for different projects.

---

# 📘 Day 3 – Solving Quadratic Equations in Python

On Day 3 of the **30-Day Algebra in Python Challenge**, I explored:

---

## 🧠 Concepts Covered

1. **Understand the Standard Form**  
   Quadratic equations are written as `ax² + bx + c = 0`

2. **Solve Quadratics with Two Real Roots**  
   Example: `x² - 5x + 6 = 0` → Roots: `2, 3`

3. **Solve Quadratics with Complex Roots**  
   Example: `x² + 4x + 5 = 0` → Roots: `-2 ± i`

4. **Solve Perfect Square Trinomials**  
   Example: `x² - 4x + 4 = 0` → Root: `2`

5. **Use SymPy to Handle All Cases**  
   Easily solve all types with `Eq()` and `solve()`

---

## 💻 Code Snippets

python
from sympy import symbols, Eq, solve

x = symbols('x')

# Two real roots
eq1 = Eq(x**2 - 5*x + 6, 0)
print("Equation 1:", eq1)
print("Solutions 1:", solve(eq1))

# Two complex roots
eq2 = Eq(x**2 + 4*x + 5, 0)
print("\nEquation 2:", eq2)
print("Solutions 2:", solve(eq2))

# One repeated root
eq3 = Eq(x**2 - 4*x + 4, 0)
print("\nEquation 3:", eq3)
print("Solutions 3:", solve(eq3))
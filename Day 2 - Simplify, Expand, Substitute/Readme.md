# 📘 Day 2 – Simplify, Expand & Substitute in Python

On Day 2 of the **30-Day Algebra in Python Challenge**, I explored:

---

## 🧠 Concepts Covered

1. **Simplify Expressions**  
   Combine like terms:  
   `2x + 3x - 4 + x → 6x - 4`

2. **Expand Binomials**  
   Multiply expressions:  
   `(x + 2)(x - 3) → x² - x - 6`

3. **Expand Powers**  
   Expand squared terms like:  
   `(2x + 1)^2 → 4x² + 4x + 1`

4. **Substitute Single Value**  
   Plug in values like `x = 2` into expressions

5. **Substitute Multiple Variables**  
   Substitute `x = 2`, `y = 3` into multivariable expressions

---

## 💻 Code Snippets

```python
from sympy import symbols, simplify, expand

x, y = symbols('x y')

# Simplify
expr1 = 2*x + 3*x - 4 + x
print("Simplified:", simplify(expr1))

# Expand binomial
expr2 = (x + 2)*(x - 3)
print("Expanded:", expand(expr2))

# Expand power
expr3 = (2*x + 1)**2
print("Expanded Power:", expand(expr3))

# Substitute single value
expr4 = x**2 + 5*x + 6
print("Substitute x=2:", expr4.subs(x, 2))

# Substitute multiple values
expr5 = x**2 + y**2 + 2*x*y
print("Substitute x=2, y=3:", expr5.subs({x: 2, y: 3}))
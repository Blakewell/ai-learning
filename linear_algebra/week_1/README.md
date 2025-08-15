# Week 1

Linear algebra materials for week 1.

## Concepts Covered

### Linear vs. Non-Linear Systems

**Linear Systems:**
- Systems where the relationship between variables can be expressed as straight lines
- Follow the principle of superposition (the output is proportional to the input)
- Can be represented by equations of the form: ax + by + c = 0
- When graphed, create straight lines, planes, or hyperplanes

**Non-Linear Systems:**
- Systems where the relationship between variables cannot be expressed as straight lines
- Do not follow the principle of superposition
- Include equations with powers, products of variables, trigonometric functions, etc.
- When graphed, create curves, parabolas, circles, or other non-linear shapes

**Key Differences:**
- Linear systems are easier to solve and analyze
- Non-linear systems can exhibit more complex behaviors
- Many real-world problems start as non-linear but can be approximated as linear for analysis

### Examples

**Linear System Examples:**
```
2x + 3y = 6
x - y = 1

Matrix form:
[2  3] [x]   [6]
[1 -1] [y] = [1]
```

```
3x + 2y - z = 5
x + y + z = 6
2x - y + 3z = 4

Matrix form:
[3  2 -1] [x]   [5]
[1  1  1] [y] = [6]
[2 -1  3] [z]   [4]
```

**Non-Linear System Examples:**
```
x² + y² = 25    (circle)
xy = 6          (hyperbola)
```

```
x² + 2xy + y² = 9
x³ - y = 2
```

Note: Non-linear systems cannot be represented in standard matrix form Ax = b because they contain non-linear terms (powers, products of variables).

### Matrices vs. Vectors

**Matrices:**
- Rectangular arrays of numbers arranged in rows and columns
- Can be of size m × n (m rows, n columns)
- Used to represent coefficients in systems of linear equations
- Example: A 3×2 matrix has 3 rows and 2 columns

**Vectors:**
- Special case of matrices with either one row or one column
- Column vector: n × 1 matrix (n rows, 1 column)
- Row vector: 1 × n matrix (1 row, n columns)
- Represent variables or constants in linear systems

**Example:**
```
Matrix A (3×3):        Vector x (3×1):        Vector b (3×1):
[2  1 -1]              [x₁]                   [8]
[1  3  2]              [x₂]                   [13]
[3 -1  1]              [x₃]                   [7]
```

### Solution Types for Linear Systems

When solving a system of linear equations Ax = b, there are three possible outcomes:

**1. Unique Solution:**
- Exactly one solution exists
- The system is consistent and the coefficient matrix has full rank
- Graphically: lines/planes intersect at exactly one point

**2. Infinite Solutions:**
- Infinitely many solutions exist
- The system is consistent but has dependent equations (redundant information)
- Graphically: lines/planes coincide or intersect along a line/plane

**3. No Solution:**
- No solution exists
- The system is inconsistent
- Graphically: parallel lines/planes that never intersect

**Determining Solution Type:**
- Compare the rank of coefficient matrix A with the rank of augmented matrix [A|b]
- If rank(A) = rank([A|b]) = number of variables → unique solution
- If rank(A) = rank([A|b]) < number of variables → infinite solutions  
- If rank(A) < rank([A|b]) → no solution
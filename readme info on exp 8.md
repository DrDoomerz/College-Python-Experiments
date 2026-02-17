# Experiment 8: Study of For Loop in Python

## Aim

To study and implement the **for loop in Python** and understand how it is used to iterate over sequences like ranges, lists, and strings.

---

# Theory

A **for loop** in Python is used to repeat a block of code for every element in a sequence.  
It is mainly used when the number of iterations is known in advance.

A sequence can be:
- Range of numbers  
- List  
- String  
- Tuple  
- Matrix (nested lists)

## Syntax of For Loop

```python
for variable in sequence:
    statements
```

Example:

```python
for i in range(1,6):
    print(i)
```

This prints numbers from 1 to 5.

## Important Concepts

###  1. range() Function
`range()` generates a sequence of numbers.

Forms:
- `range(stop)`
- `range(start, stop)`
- `range(start, stop, step)`

Example:
```python
range(1,10,2)  # prints odd numbers
```

### 2. Nested For Loops
A loop inside another loop.  
Used for:
- Matrix operations  
- Pattern printing  
- Combinations

### 3. Loop Control
- `break` → exits loop  
- `continue` → skips current iteration  

### 4. Real-Life Uses
- Matrix multiplication  
- Generating combinations  
- Pattern design  
- Prime number generation  
- Summation problems  

For loops are essential for structured iteration in programming.

---

# Algorithms (DIY Programs Only)

## 🔹 DIY 1: Sum of First N Numbers

**Algorithm**

1. Input value of N.  
2. Initialize sum = 0.  
3. Loop from 1 to N.  
4. Add each number to sum.  
5. Print sum.

---

## 🔹 DIY 2: Print Matrix

**Algorithm (Method 1)**  
1. Define matrix.  
2. Loop through each row.  
3. Loop through each element.  
4. Print elements row-wise.

**Algorithm (Method 2)**  
1. Define matrix.  
2. Loop through rows.  
3. Print each row directly.

---

## 🔹 DIY 3: Matrix Multiplication

**Algorithm**

1. Define matrices A and B.  
2. Initialize result matrix with zeros.  
3. Use three nested loops.  
4. Multiply corresponding elements.  
5. Add results to result matrix.  
6. Print result.

---

## 🔹 DIY 4: Number Combinations

**Algorithm**

1. Store numbers in list.  
2. Use three nested loops.  
3. Ensure digits are not repeated.  
4. Print valid combinations.

---

## 🔹 DIY 5: Right Angled Triangle

**Algorithm (Method 1)**  
1. Loop from higher value to lower.  
2. Print stars each time.

**Algorithm (Method 2)**  
1. Input rows.  
2. Outer loop controls rows.  
3. Inner loop prints stars.  
4. Move to next line.

---

## 🔹 DIY 6: Pyramid Pattern

**Algorithm**

1. Set number of rows.  
2. Loop from 1 to rows.  
3. Print spaces.  
4. Print stars.  
5. Repeat.

---

## 🔹 DIY 7: Prime Numbers

**Algorithm**

1. Loop from 2 to 50.  
2. For each number, check divisibility.  
3. If divisible → not prime.  
4. If not divisible → print number.

---

# Conclusion

In this experiment, the **for loop** was studied and implemented for different applications like summation, matrix operations, combinations, pattern printing, and prime number generation.

This experiment helped in:
- Understanding iteration  
- Improving logical thinking  
- Learning nested loops  
- Applying loops to real problems  

For loops are a fundamental tool in Python programming and widely used in practical applications.

---

# 👨‍💻 Author

**Rachit Jajoo**  
Electronics & Telecommunication Engineering (ENTC)  
Symbiosis Institute of Technology, Pune

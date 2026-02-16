# Experiment 7: Study of While Loop in Python

## Aim

To study and understand the **while loop in Python** and use it to perform repetitive tasks where the number of iterations is not known beforehand.

---

# Theory

A **loop** in programming is used to repeat a block of code multiple times.  
Among loops in Python, the **while loop** is used when we do not know in advance how many times the loop should run.

The loop continues to execute as long as the given condition is **True**.

### Syntax

```python
while condition:
    statement(s)
```

The condition is checked before every iteration.  
If it becomes False, the loop stops.

## Key Concepts of While Loop

### 1. Condition-Controlled Loop
A while loop runs based on a condition.  
It stops only when the condition becomes False.

### 2. Initialization and Updation
- A variable must be initialized before the loop.
- The variable must be updated inside the loop.
- Otherwise, the loop may run forever (infinite loop).

### 3. Infinite Loop
If the condition never becomes False, the loop runs infinitely.  
Example:

```python
while True:
    print("Hello")
```

### 4. break Statement
Used to immediately exit the loop even if the condition is True.

### 5. continue Statement
Skips the current iteration and moves to the next one.

## 💡 Real-Life Importance

While loops are useful in:
- Factorial calculations  
- Fibonacci series  
- Palindrome checks  
- Digit counting  
- Searching in lists  
- Reversing numbers  
- Input validation systems  

They are essential for building logical thinking in programming.

---

# Algorithms (DIY Programs)

---

## 🔹 DIY 1: Factorial of a Number

**Algorithm**

1. Input a non-negative integer.  
2. Initialize factorial = 1 and i = 1.  
3. Repeat while i ≤ number.  
4. Multiply factorial by i.  
5. Increment i.  
6. Display factorial.

---

## 🔹 DIY 2: Fibonacci Series (Method 1)

**Algorithm**

1. Input number of terms.  
2. Initialize n1 = 0, n2 = 1, count = 0.  
3. While count < terms:  
   - Print n1  
   - Compute next term  
   - Update values  
   - Increase count.

---

## 🔹 DIY 2 (Method 2): Fibonacci Series

**Algorithm**

1. Input number of terms.  
2. Initialize a = 0, b = 1, i = 1.  
3. While i ≤ terms:  
   - Print a  
   - Compute next value  
   - Update a and b  
   - Increment i.

---

## 🔹 DIY 3: Fibonacci Series up to Limit

**Algorithm**

1. Input limit.  
2. Initialize a = 0, b = 1.  
3. While a ≤ limit:  
   - Print a  
   - Update a and b.

---

## 🔹 DIY 4: Reverse a Number

**Algorithm**

1. Input number.  
2. Initialize reversed = 0.  
3. While number > 0:  
   - Get last digit  
   - Add to reversed  
   - Remove last digit.  
4. Display reversed number.

---

## 🔹 DIY 5: Palindrome Number

**Algorithm**

1. Input number.  
2. Reverse the number.  
3. Compare original and reversed.  
4. If equal → Palindrome.  
5. Else → Not palindrome.

---

## 🔹 DIY 5 (Part 2): Palindrome String

**Algorithm**

1. Input string.  
2. Reverse string using loop.  
3. Compare original and reversed.  
4. Print result.

---

## 🔹 DIY 6: Count Digits in Number

**Algorithm**

1. Input number.  
2. Initialize count = 0.  
3. While number > 0:  
   - Divide number by 10  
   - Increase count.  
4. Display count.

---

## 🔹 DIY 6: Search Element in List

**Algorithm**

1. Create list.  
2. Input element to search.  
3. Start from index 0.  
4. Compare each element.  
5. If found → print index and stop.  
6. Else → print not found.

---

## 🔹 DIY 7: Print Odd Numbers (1–10)

**Algorithm**

1. Initialize i = 0.  
2. While i < 10:  
   - Increase i  
   - If even → continue  
   - Else print.

---

# Conclusion

In this experiment, the working of the **while loop** was studied and implemented.  
Various programs such as factorial, Fibonacci series, palindrome check, digit counting, and list searching were performed.

This experiment improved:
- Logical thinking  
- Understanding of loops  
- Problem-solving skills  
- Flow control knowledge  

The while loop proved to be powerful for solving problems where the number of iterations is not fixed.

---

# 👨‍💻 Author

**Rachit Jajoo**  
ENTC Engineering  
Symbiosis Institute of Technology, Pune

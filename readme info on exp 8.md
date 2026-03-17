# Experiment 8: Study of For Loop in Python

## Aim

To study the **usage of the for loop in Python** and implement it for various operations such as number generation, summation, matrix handling, pattern printing, combinations, and prime number generation.

---

## Theory

A **for loop** in Python is a control flow statement used to execute a block of code repeatedly for each element present in a sequence. It is particularly useful when the number of iterations is known beforehand or when traversing through structured data.

Unlike some other programming languages, Python’s `for` loop works directly with sequences rather than relying only on counters.

### General Syntax

```python
for variable in sequence:
    statements
````

Where:

* **variable** takes the value of each element in the sequence
* **sequence** can be any iterable object
* **statements** are executed repeatedly for each element

---

## Types of Sequences Used

1. **Range**

   * Generates a sequence of numbers
   * Commonly used for looping a fixed number of times

   ```python
   range(start, stop, step)
   ```

2. **List**

   * Stores multiple values
   * Loop accesses elements one by one

3. **String**

   * Loop iterates through each character

4. **Matrix (Nested List)**

   * Multi-dimensional structure
   * Requires nested loops

---

## Key Concepts of For Loop

### 1. Iteration using range()

Controls how many times the loop runs.

```python
for i in range(2, 11, 2):
    print(i)
```

---

### 2. Conditional Statements inside Loop

Used to filter values during iteration.

```python
if i % 2 == 0:
    print(i)
```

---

### 3. Nested For Loop

A loop inside another loop.

Used in:

* Matrix operations
* Pattern printing
* Combinational problems

---

### 4. Accumulator Pattern

Used to compute sum or product.

```python
sum = 0
for i in range(1,6):
    sum += i
```

---

### 5. Loop Control Statements

* `break` → terminates loop
* `continue` → skips iteration

---

## Applications of For Loop

* Number generation
* Summation problems
* Matrix traversal and multiplication
* Pattern printing
* Combinations generation
* Prime number generation

---

## Algorithms

---

### 🔹 DIY 1: Sum of First N Numbers

**Algorithm**

1. Start the program.
2. Accept an integer input **N** from the user.
3. Initialize a variable `sum = 0` to store the result.
4. Use a `for` loop to iterate from **1 to N (inclusive)** using `range(1, N+1)`.
5. For each iteration:

   * Add the current value of `i` to `sum`.
   * Update the value of `sum`.
6. After completion of the loop, display the value of `sum`.
7. End the program.

---

### 🔹 DIY 2: Print Matrix

#### Method 1 (Element-wise Printing)

**Algorithm**

1. Start the program.
2. Define a 2D list (matrix) with rows and columns.
3. Use an outer `for` loop to iterate through each row of the matrix.
4. Inside the outer loop, use an inner `for` loop to iterate through each element of the row.
5. Print each element using `end=" "` to maintain row format.
6. After printing one row, move to the next line using `print()`.
7. Repeat until all rows are printed.
8. End the program.

---

#### Method 2 (Row-wise Printing)

**Algorithm**

1. Start the program.
2. Define a matrix as a list of lists.
3. Use a `for` loop to iterate through each row.
4. Print the entire row directly.
5. Repeat for all rows.
6. End the program.

---

### 🔹 DIY 3: Matrix Multiplication (3×3)

**Algorithm**

1. Start the program.
2. Define two matrices **A** and **B** of size 3×3.
3. Initialize a result matrix **Result** with all elements as 0.
4. Use three nested loops:

   * Outer loop for rows (`i`)
   * Middle loop for columns (`j`)
   * Inner loop for multiplication (`k`)
5. For each element:

   * Multiply corresponding elements: `A[i][k] * B[k][j]`
   * Add the result to `Result[i][j]`
6. Repeat until all elements are computed.
7. Display the final result matrix.
8. End the program.

---

### 🔹 DIY 4: Number Combinations

**Algorithm**

1. Start the program.
2. Initialize three digits and store them in a list.
3. Use three nested loops to generate combinations:

   * First loop selects first digit
   * Second loop selects second digit
   * Third loop selects third digit
4. Inside the innermost loop:

   * Check that all digits are distinct using conditions
     `(d[i] != d[j] and d[j] != d[k] and d[i] != d[k])`
5. If condition is satisfied:

   * Print the combination
6. Repeat until all possible combinations are generated.
7. End the program.

---

### 🔹 DIY 5: Right Angled Triangle Pattern

#### Method 1 (Decreasing Pattern)

**Algorithm**

1. Start the program.
2. Use a `for` loop from a higher value to 1 (reverse order).
3. In each iteration:

   * Print `"* "` multiple times equal to loop value.
4. Move to the next line after each iteration.
5. Repeat until pattern completes.
6. End the program.

---

#### Method 2 (Increasing Pattern)

**Algorithm**

1. Start the program.
2. Accept number of rows as input.
3. Use an outer loop to control rows.
4. Use an inner loop to print stars:

   * Print stars equal to current row number (`i+1`)
5. Move to next line after each row.
6. Repeat until all rows are printed.
7. End the program.

---

### 🔹 DIY 6: Pyramid Pattern

**Algorithm**

1. Start the program.
2. Set number of rows.
3. Use a loop from 1 to number of rows.
4. For each row:

   * Print spaces to align pyramid: `(rows - i)`
   * Print stars: `i` times
5. Combine spaces and stars in one print statement.
6. Move to next line after each row.
7. Repeat until pyramid is complete.
8. End the program.

---

### 🔹 DIY 7: Prime Number Generation

**Algorithm**

1. Start the program.
2. Use a loop to iterate numbers from **2 to 50**.
3. For each number:

   * Assume it is prime initially.
4. Use another loop to check divisibility from **2 to (num-1)**.
5. If the number is divisible:

   * Use `break` to exit loop (not prime).
6. If loop completes without break:

   * Print the number as prime.
7. Repeat for all numbers.
8. End the program.

---

## Conclusion

In this experiment, the **for loop in Python** was thoroughly studied and implemented using multiple examples and problem statements.

The experiment helped in:

* Understanding iteration over different data structures
* Learning the use of `range()` and conditional statements
* Implementing nested loops for complex problems
* Performing matrix operations and pattern generation
* Developing logical thinking through combinational and prime number problems

Thus, the **for loop is a powerful and essential construct** in Python programming.

---

## 👨‍💻 Author

**Rachit Jajoo**
Electronics & Telecommunication Engineering (ENTC)
Symbiosis Institute of Technology, Pune

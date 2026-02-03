# Experiment 3: Study of Tuples in Python

## Aim

To study the concept of **tuples in Python** and understand their properties and usage through basic programs and DIY problem statements.

---

## Theory

A **tuple** in Python is an ordered collection of elements enclosed in parentheses `()`. Tuples can store elements of different data types such as integers, floats, and strings.

### Features of Tuples

* **Ordered:** Elements have a fixed position.
* **Immutable:** Once created, elements cannot be changed.
* **Allows duplicates:** Same values can appear multiple times.
* **Supports mixed data types.**

Example:

```
t = (10, "apple", 3.5)
```

### Tuple Operations

* **Indexing:** Access elements using position numbers.
* **Slicing:** Extract a part of a tuple using `start:end`.
* **Concatenation:** Combine tuples using `+`.
* **Repetition:** Repeat elements using `*`.
* **Length:** `len()` gives number of elements.
* **Built-in functions:** `max()`, `min()`, and `sum()` work on numeric tuples.

### Tuple Packing and Unpacking

Tuple packing means storing multiple values in one tuple. Unpacking means assigning tuple elements to variables.

Example:

```
student = ("Math", 85, "A")
sub, marks, grade = student
```

Tuples are useful when data should remain constant and not be modified accidentally.

---

## Algorithms (DIY Questions Only)

### DIY Problem 1: Student Marks Analysis

**Steps:**

1. Create a tuple containing marks of students.
2. Use `max()` to find highest marks.
3. Use `min()` to find lowest marks.
4. Use `len()` to find total students.
5. Use `sum()` to find total marks.
6. Calculate average using total marks divided by number of students.
7. Display all results.

---

### DIY Problem 2: Student Result Evaluation

**Steps:**

1. Create a tuple containing subject name, marks, and grade.
2. Unpack the tuple into three variables.
3. Display subject, marks, and grade separately.
4. Check if marks are 75 or more.
5. Print "Distinction" if condition is satisfied.

---

### DIY Problem 3: Attendance Record Analysis

**Steps:**

1. Create a tuple storing attendance using "P" and "A".
2. Count number of "P" for present days.
3. Count number of "A" for absent days.
4. Check if "A" exists in the tuple.
5. Display appropriate attendance message.

---

## Conclusion

In this experiment, tuples in Python were studied and implemented. Tuple creation, indexing, slicing, packing, and unpacking were understood. The DIY problems showed how tuples can be used in real-life situations like marks analysis and attendance tracking. This experiment helped in understanding the importance of immutable data structures in Python.

---

**Author:** Rachit Jajoo
**Branch:** Electronics and Telecommunication Engineering (ENTC)
**Institute:** Symbiosis Institute of Technology, Pune

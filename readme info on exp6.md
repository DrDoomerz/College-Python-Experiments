#  Experiment 6: Study of Conditional Statements in Python

## Aim

To study and implement **conditional statements in Python** using `if`, `if-else`, and `if-elif-else` constructs for decision-making operations.

---

#  Theory

Conditional statements in Python are used for **decision making**. They allow a program to execute specific code blocks based on whether a condition is true or false.

---

##  1. if Statement

The `if` statement executes a block of code only when the condition is true.

```python
if condition:
    statement
```

---

##  2. if-else Statement

Used when there are two possible outcomes:

- If condition is true → first block executes  
- If false → second block executes  

---

##  3. if-elif-else Statement

Used when multiple conditions are checked.

Python evaluates conditions from top to bottom and executes the first true condition.

---

##  4. Comparison Operators

| Operator | Meaning |
|--------|--------|
| `>` | Greater than |
| `<` | Less than |
| `>=` | Greater or equal |
| `<=` | Less or equal |
| `==` | Equal to |
| `!=` | Not equal to |

---

##  5. Logical Operators

| Operator | Use |
|--------|------|
| `and` | Both conditions must be true |
| `or` | At least one true |
| `not` | Reverses condition |

---

##  6. Importance of Indentation

Python uses indentation to define code blocks.  
Incorrect indentation results in errors.

---

##  7. Applications of Conditional Statements

- Positive/Negative number check  
- Even/Odd detection  
- Grade calculation  
- Salary computation  
- Income tax calculation  
- Date validation  
- Vowel/Consonant check  

Conditional statements help simulate real-life decision making in programs.

---

#  Algorithms (DIY Questions Only)

---

## 🔹 DIY 1: Leap Year Check

**Algorithm**

1. Input year from user  
2. Check if divisible by 400  
3. OR divisible by 4 but not by 100  
4. If true → Leap year  
5. Else → Not a leap year  

---

## 🔹 DIY 2: Date Increment Program

**Algorithm**

1. Input date in `dd/mm/yyyy` format  
2. Split into day, month, year  
3. Convert to integers  
4. Determine max days in month  
5. Check leap year for February  
6. Validate date  
7. If last day → reset day & increment month  
8. If 31 Dec → increment year  
9. Else increment day  
10. Display new date  

---

## 🔹 DIY 3: Gross Salary Calculation

**Algorithm**

1. Input basic salary  
2. If ≤10000 → HRA 20%, DA 80%  
3. If ≤20000 → HRA 25%, DA 90%  
4. Else → HRA 30%, DA 95%  
5. Gross = Basic + HRA + DA  
6. Display salary  

---

## 🔹 DIY 4: Income Tax Calculation

**Algorithm**

1. Input annual salary  
2. ≤250000 → No tax  
3. ≤500000 → 5% above 250000  
4. ≤1000000 → 20% above 500000 + previous tax  
5. Else → 30% above 1000000 + previous slabs  
6. Display tax  

---

## 🔹 DIY 5: Vowel or Consonant Check

**Algorithm**

1. Input character  
2. Check if vowel  
3. If yes → Print vowel  
4. Else check consonant  
5. If yes → Print consonant  
6. Else → Invalid  

---

#  Conclusion

This experiment helped in understanding **conditional statements** in Python.  
Programs using `if`, `if-else`, and `if-elif-else` were implemented for logical decision-making.

The DIY problems demonstrated real-life applications such as:

- Leap year detection  
- Date validation  
- Salary & tax calculation  
- Character classification  

This experiment strengthened logical thinking and programming skills.

---

# 👨‍💻 Author

**Rachit Jajoo**  
Electronics & Telecommunication Engineering (ENTC)  
Symbiosis Institute of Technology, Pune

# Experiment 4: Study of Sets in Python

## Aim

To study the concept of **sets in Python** and perform different operations on sets using simple programs.

---

## Theory

A **set** in Python is a collection used to store multiple items in a single variable. Sets are written using curly brackets `{}`.

Important points about sets:

* Sets are **unordered** (items do not have a fixed position)
* Sets are **unindexed** (no indexing or slicing)
* Sets do **not allow duplicate values**
* Sets are **mutable**, meaning we can add or remove items
* Sets can store different data types

### Basic Set Concepts Covered

**1. Creation of Set**
A set can be created using curly braces with comma-separated values.

**2. No Duplicates**
If duplicate values are entered, they are automatically removed.

**3. Boolean and Numeric Equality**
`True` and `1` are treated as the same value in sets.

**4. Membership Test**
The `in` keyword is used to check whether an element exists in a set.

**5. Adding Elements**
`add()` is used to add new items to a set.

**6. Removing Elements**
`remove()` or `discard()` is used to delete items.

**7. Set Operations**

* Union (`|`)
* Intersection (`&`)
* Difference (`-`)
* Symmetric Difference (`^`)
* Subset and Superset checks

**8. Frozenset**
A frozenset is an immutable version of a set where elements cannot be added or removed.

---

## Algorithms (Problem Statements Only)

### Problem Statement 1: Unique Event Participants

**Steps:**

1. Create a list of participant names containing duplicates.
2. Convert the list into a set.
3. Display the set to show only unique participants.

---

### Problem Statement 2: Common Elective Subjects

**Steps:**

1. Create three sets for subjects chosen by students.
2. Use intersection operation to find common subjects.
3. Display the common subjects.

---

### Problem Statement 3: Students in Sports Clubs

**Steps:**

1. Create two sets for cricket and football club members.
2. Use intersection to find students in both clubs.
3. Use symmetric difference to find students in only one club.
4. Display the results.

---

### Problem Statement 4: Absent Students

**Steps:**

1. Create a set of all students.
2. Create a set of present students.
3. Use set difference to find absent students.
4. Display the absent students.

---

### Problem Statement 5: Remove Invalid Course Code

**Steps:**

1. Create a set of valid course codes.
2. Identify the discontinued code.
3. Use `discard()` to remove it from the set.
4. Display the updated set.

---

## Conclusion

In this experiment, the concept of sets in Python was studied. Various properties like uniqueness, unordered nature, and mutability were understood. Operations such as union, intersection, and difference were performed. Real-life problem statements helped in applying the concept practically. This experiment improved understanding of how sets are useful for handling unique data and performing group-based operations.

---

**Author:** Rachit Jajoo
**Branch:** Electronics and Telecommunication Engineering (ENTC)
**Institute:** Symbiosis Institute of Technology, Pune

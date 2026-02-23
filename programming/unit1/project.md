# Unit 1 Programming Assignment

## Create-Your-Own Calculator Program

---

## Overview

For this assignment, you will design and build your own interactive Python program.

Your program must:

* Ask the user for input
* Store data in variables
* Perform mathematical calculations
* Display organized output
* Demonstrate all Unit 1 concepts

You may choose **any appropriate scenario** as long as it involves numbers and calculations.

---

## Choose Your Scenario

You may create a program such as:

* Shopping total calculator
* Sports statistics calculator
* Road trip cost estimator
* Gaming score calculator
* Party budget planner
* Restaurant bill calculator
* Pet care cost calculator
* Fitness tracker
* Concert ticket calculator
* Allowance savings calculator

Or create your own idea (school appropriate).

Your program must include:

* **At least 3 user inputs**
* **At least 4 mathematical calculations**

---

## Required Concepts Checklist

Your program must clearly demonstrate **all** of the following:

---

### 1. Program Header (Required)

At the top of your file:

```python
# Program: (Your Program Name)
# Name: (Your Name)
# Date:
# Description: (1–2 sentence explanation of what your program does)
```

---

### 2. Comments

Include:

* At least **3 meaningful comments** explaining parts of your code
* Not just “# this is a variable”

---

### 3. Variables and Data Types

Your program must include:

* At least **2 integers**
* At least **2 floats**
* At least **2 strings**

You must:

* Assign values to variables
* Follow proper variable naming rules:

  * No spaces
  * Cannot start with a number
  * No special characters (except underscore)
  * Use meaningful names

---

### 4. Input Function

You must:

* Use `input()` with a prompt
* Demonstrate that input returns a string
* Use `int()` and `float()` to cast values for calculations

Example:

```python
quantity = int(input("How many items? "))
price = float(input("Enter the price: "))
```

---

### 5. Printing Requirements

You must:

* Use `print()`
* Use commas in at least one print statement
* Use `\n` to organize output
* Use string concatenation at least once
* Demonstrate proper casting when concatenating

Example:

```python
print("\n----- RESULTS -----")
print("Total cost:", total)
print("Final cost is $" + str(total))
```

---

### 6. Math Operators

Your program must use **all** of these operators somewhere in the program:

* `+`
* `-`
* `*`
* `/`
* `//`
* `%`
* `**`

Not all have to be central to the scenario — some can be demonstrated creatively.

Examples:

* Use `//` and `%` to break money into bills and leftover change
* Use `**` to square a number
* Use `/` to calculate an average
* Use `*` to calculate totals

---

### 7. Expressions

You must use at least **2 multi-step expressions**.

Example:

```python
total = (price * quantity) - discount
```

---

## Common Mistakes to Avoid

* Forgetting to cast input before math
* Trying to concatenate a string and integer without `str()`
* Missing required operators
* Not including `\n`
* Weak or missing comments
* Poor variable names like `x`, `a`, or `thing`

---

## Extra Credit (Optional)

* Add a discount system
* Add tax
* Personalize output with the user’s name
* Add decorative formatting
* Add a second calculation section

---

## What This Assignment Demonstrates

By completing this project, you demonstrate:

* Understanding of data types
* Proper variable usage
* Safe casting
* Expression evaluation
* Operator knowledge
* Organized program structure
* Clean, readable code

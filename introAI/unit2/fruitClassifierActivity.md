# 🍎 Activity: “Is This a Fruit?” – Classifier Challenge

### 🎯 Objective

Design a rule-based system to classify fruits from a **pre-defined list**. Then test your system with a partner and try to find weaknesses in each other’s rules.

---

## 📝 Part 1: Choose Your Target Fruit

Select **one fruit from this list**:

* Apple
* Banana
* BlackBerry
* Cantaloupe
* Cherry
* Grape
* Orange
* Papaya
* Peach
* Pear
* Raspberry
* Strawberry

> ⚠️ Some fruits may look similar or have variants — this will make your rules more interesting!

---

## 🧾 Part 2: Define Your Category

Write a clear definition:

* What counts as **YES** (your target fruit)?
* What counts as **NO** (anything else on the list)?

---

## 📏 Part 3: Build Your Rule System

You must create **6–8 rules minimum**.

### Your rules must include at least:

* ✅ **2 YES rules** – features that must be true for it to be classified as your fruit
* ❌ **2 NO rules** – features that automatically disqualify it


⚖️ Dont' forget about **edge cases** – the tricky situations outside of the "norm" (like different colors, sizes, or shapes)

### Rule Guidelines:

* Be **clear and specific**
* Base rules on **observable features**
* Avoid vague language (no “looks like a fruit” or “seems sweet”)

---

## 🔄 Part 4: Exchange and Test

1. Swap your rules with a classmate.
2. Use the **random fruit image webpage** to test each other’s classifier.
    * Go to the webpage and show a random fruit
    * For every fruit, read the rules and determine if the fruit on the webpage is the classifier's target fruit.
    * Record yes or no, then reveal the fruit on the webpage to check if the classifier classified the fruit correctly. Record the result
    * Write the name of the fruit under the `Image` heading below
    * Do this for a minimum of 10 fruits
3. Record results:

| Image | YES/NO | Correct? | Notes |
| ----- | ------ | -------- | ----- |
|       |        |          |       |

<br>
<br>
<br>
<br>
<br>
<br>
---

## ⚠️ Part 5: Find Failures

Look for:

* ❌ False Positives (wrongly classified as YES)
* ❌ False Negatives (wrongly classified as NO)

Answer:

* Which images broke the rules?
* Which rules caused mistakes?
* Are any rules unclear or conflicting?

---

## 🔧 Part 6: Improve Your Rules

* ➕ Add at least **2 new rules**
* 🔁 Modify at least **2 existing rules**

Then retest.

---

## 🧪 Example

### Target Fruit: Tomato

**Definition:** medium, round fruit, red, yellow, or green variants, with seeds inside.

**Rules:**

* **YES:**

  * Round shape
  * Red, yellow, or green color

* **NO:**

  * Grows underground
  * Has multiple small seeds on the outside

* **Edge Cases:**

  * Small variant → still count as cherry tomato
  * If shown on a vine → still count as tomato

**Test Examples:**

| Image     | YES/NO | Correct?  |
| --------- | ------ | --------- |
| Tomato    | Yes    | ✅         |
| Grape     | NO     | ✅         |
| Cherry    | NO     | 🤔 debate |
| Raspberry | NO     | ✅         |

> Clear rules and edge-case handling are important.

---

## 🧩 Reflection

* Were your rules ever perfect? Why or why not?
* Which fruits were hardest to classify?
* Did edge cases break your rules?
* How did testing with your partner improve your system?

---

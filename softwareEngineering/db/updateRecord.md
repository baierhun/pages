# ✏️ Lanterna Project – Add Update Functionality

Your application currently allows users to **create, view, and delete records** in your database. Now it’s time to complete the CRUD cycle by adding the **Update** feature.

## 🎯 Objective

Add functionality to your app that allows a user to **edit and update an existing record** in the database.

This must:

* Modify data already stored in the database
* Use a proper SQL `UPDATE` statement
* Work through your existing UI

---

## ✅ Requirements

You must implement **at least one working way** to update a record. Some suggested approaches:

* ✔ Option A: Add an **Edit option when listing records**
* ✔ Option B: Add an **Edit button when viewing an individual record**
* ✔ Option C: Implement both (recommended, but not required)

Somewhere in your app, a user must be able to edit and save changes to a record.

---

## 🧠 Implementation Guidelines

### 1. SQL

You will need to use a parameterized query:

```sql
UPDATE your_table
SET column1 = ?, column2 = ?, column3 = ?
WHERE id = ?
```

Do **NOT** concatenate values into the SQL string.

---

### 2. Editing Flow (Required)

A typical update flow should look like this:

1. User selects a record to edit
2. A form appears with the **current values pre-filled**
3. User modifies one or more fields
4. User submits/saves changes
5. Database is updated

---

### 3. Validation (Required)

Before updating:

* Ensure required fields are not empty
* Prevent invalid data (based on your app’s rules)

---

### 4. After Update

After a record is updated:

* The UI should reflect the changes

  * Return to the list
  * Refresh the view
  * Or show a success message

The updated values should be visible immediately.

---

## 💡 What We’re Looking For

* Correct SQL usage (`UPDATE`)
* Proper use of PreparedStatement
* Pre-filled edit form
* Smooth user experience
* Data validation before saving
* No crashes if the user enters bad input

---

## 🚫 Common Mistakes to Avoid

* Forgetting the `WHERE` clause (this updates EVERYTHING 😬)
* Not pre-filling the form with existing data
* Losing the record’s ID during editing
* Not validating user input
* UI not reflecting updated data
* Not closing database resources

---

## 📦 Submission Instructions

1. Commit your changes locally.
2. Push to GitHub.
3. Go to your repository on GitHub.
4. Click on your most recent commit.
5. Copy the **commit URL**.
6. Submit that URL to Canvas.

You are submitting the **commit link**.

---

## 🏆 Goal

After this assignment, your app should now support:

* Create
* Read
* Update
* Delete

🎉 Full CRUD functionality!

---

## 📊 Grading (15 Points Total)

### 1️⃣ Update Function Works (6 points)

* 6 pts — Record is correctly updated in the database.
* 3–5 pts — Partially works or inconsistent.
* 0 pts — Does not update database.

---

### 2️⃣ Proper SQL + PreparedStatement (3 points)

* 3 pts — Uses parameterized `UPDATE` with `?`.
* 1–2 pts — Minor issues.
* 0 pts — Unsafe string concatenation or incorrect SQL.

---

### 3️⃣ UI Integration (2 points)

* 2 pts — Edit flow is clear and intuitive.
* 1 pt — Exists but awkward/confusing.
* 0 pts — Poor or broken integration.

---

### 4️⃣ Pre-Filled Form (2 points)

* 2 pts — Fields are correctly pre-populated with existing data.
* 1 pt — Partially filled or inconsistent.
* 0 pts — Blank form (user must retype everything).

---

### 5️⃣ Validation (1 point)

* 1 pt — Prevents invalid or empty data.
* 0 pts — No validation.

---

### 6️⃣ Clean Commit & Submission (1 point)

* 1 pt — Proper commit pushed and correct commit URL submitted.
* 0 pts — No valid commit link.

---

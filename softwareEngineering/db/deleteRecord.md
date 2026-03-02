# 🗑️ Lanterna Project – Add Delete Functionality

Your application currently allows users to **create and view records** in your database. Now it’s time to continue the basic CRUD cycle by adding the **Delete** feature.

## 🎯 Objective

Add functionality to your app that allows a user to **delete a record from the database**.

This must:

* Actually remove the record from the database (not just from the screen)
* Use a proper SQL `DELETE` statement
* Work through your existing UI

---

## ✅ Requirements

You must implement **at least one working way** to delete a record:

* ✔ Option A: Add a **Delete button when listing records**
* ✔ Option B: Add a **Delete button when viewing an individual record**
* ✔ Option C: Implement both (recommended, but not required)

Somewhere in your app, a user must be able to delete a record from the database.

---

## 🧠 Implementation Guidelines

### 1. SQL

You will need to use a parameterized query:

```sql
DELETE FROM your_table
WHERE id = ?
```

Do **NOT** concatenate the id into the SQL string.

---

### 2. Safety Consideration (Required)

Before deleting, you must:

* Either ask for confirmation (ex: “Are you sure?” prompt)
* OR clearly indicate which record is being deleted

We don’t want accidental deletions.

---

### 3. After Deletion

After a record is deleted:

* The UI should update appropriately

  * Return to the list
  * Or refresh the list
  * Or show a success message

The deleted record should no longer appear.

---

## 💡 What We’re Looking For

* Correct SQL usage (`DELETE`)
* Proper use of PreparedStatement
* Good UI integration
* Clean user experience
* No crashes if the user tries something unexpected

---

## 🚫 Common Mistakes to Avoid

* Deleting the wrong record
* Forgetting the `WHERE` clause (this deletes EVERYTHING 😬)
* Not closing database resources
* UI still showing deleted data

---

## 📦 Submission Instructions

1. Commit your changes locally.
2. Push to GitHub.
3. Go to your repository on GitHub.
4. Click on your most recent commit.
5. Copy the **commit URL**.
6. Submit that URL to Canvas.

You are submitting the **commit link**, not a zip file.

---

## 🏆 Goal

After this assignment, your app should now support:

* Create
* Read
* **Delete**

---

## 📊 Grading (13 Points Total)

### 1️⃣ Delete Function Works (5 points)

* 5 pts — Record is correctly deleted from the database.
* 3 pts — Partially works or inconsistent.
* 0 pts — Does not delete from database.

### 2️⃣ Proper SQL + PreparedStatement (3 points)

* 3 pts — Uses parameterized `DELETE` with `?`.
* 1–2 pts — Minor issues.
* 0 pts — Unsafe string concatenation or incorrect SQL.

### 3️⃣ UI Integration (2 points)

* 2 pts — Delete option is clearly integrated and intuitive.
* 1 pt — Exists but awkward/confusing.
* 0 pts — Poor or broken integration.

### 4️⃣ Confirmation / Safety (1 point)

* 1 pt — Confirmation prompt or clear safety measure.
* 0 pts — No protection against accidental deletion.

### 5️⃣ Clean Commit & Submission (2 points)

* 2 pts — Proper commit pushed and correct commit URL submitted.
* 1 pt — Minor submission issue.
* 0 pts — No valid commit link.
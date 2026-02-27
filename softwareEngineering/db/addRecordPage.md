# Lanterna Project – Insert Data Page

You already created a page that **retrieves and displays data** from the database.

Now you will build a second page that allows the user to **insert new records into the database** using the Lanterna GUI.

---

## 🎯 Objective

Extend your existing project by adding a new window that allows users to input data and save it to the database.

This assignment focuses on:

* Creating a new `Window`
* Using `TextBox` components for input
* Creating a `Button` with an action/listener
* Updating your **Service layer**
* Updating your **Repository layer**
* Proper Git workflow (commit → push → submit link)

---

## ✅ Requirements

### 1. Create a New Window

* Create a separate class for the new window (ex: `AddMovieWindow`, `CreateUserWindow`, etc.).
* The window must be accessible from your existing application (navigation button, menu option, etc.).
* Use appropriate layout managers.

---

### 2. Add User Input Fields

Your window must include:

* At least **two `TextBox` inputs**
* Clear labels for each field
* Logical layout and spacing

Example inputs might include:

* Name
* Title
* Year
* Email
* Description
  (Choose fields that match your project’s database.)

---

### 3. Add a Submit Button

* Add a `Button`
* Define an action/listener
* When clicked:

  * Read values from the `TextBox` components
  * Validate basic input (not empty)
  * Call a method in your **Service layer**

You may show a confirmation message after insertion.

---

### 4. Update the Service Layer

Add a new method to your service class that:

* Accepts the required data as parameters
* Performs any validation or formatting
* Calls the repository method

Example (conceptually):

```java
public void addMovie(String title, int year)
```

---

### 5. Update the Repository Layer

Add a new method that:

* Uses a `PreparedStatement`
* Executes an `INSERT INTO` query
* Properly handles exceptions
* Closes resources

Example conceptually:

```sql
INSERT INTO movie (title, release_year) VALUES (?, ?);
```

---

### 6. Database Verification

After inserting:

* You should be able to confirm the data exists by:

  * Using your existing “view results” page
  * Or checking the database directly

---

## 💻 Git Requirements

You must:

1. `git add .`
2. `git commit -m "Added insert window and database insert functionality"`
3. `git push`

Submit:

* A direct link to the commit on GitHub
  (Not just the repo link — the specific commit link.)

---

## 📋 Grading (Simple Checklist)

| Requirement                    | Points |
| ------------------------------ | ------ |
| New Window Created             | 2      |
| TextBoxes + Labels             | 2      |
| Working Button with Listener   | 2      |
| Service Method Added           | 2      |
| Repository INSERT Method       | 2      |
| Insert Successfully Works      | 2      |
| Proper Commit & Link Submitted | 1      |

**Total: 13 points**

---

If you finish early:

* Add input validation with error messages
* Clear the form after submission
* Add navigation back to the main page
* Add confirmation dialog

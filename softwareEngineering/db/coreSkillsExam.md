# **Core Skills Exam**

## **SQL \+ Lanterna Project Requirements**

For this exam, you will submit a working portion of your SQL/Lanterna project. Your submission must demonstrate that you can:

* Design a multi-screen Lanterna application

* Navigate between nested screens

* Connect to and interact with a database

---

## **Required Application Structure**

Your program must include:

### **1️⃣ Home / Menu Screen**

* This is the starting screen of your application.

* It must include menu options that allow the user to navigate to **Screen 1**.

* The Home screen does **not** need to access the database.

---

### **2️⃣ Screen 1**

* Must be accessible from the Home screen.

* Must include an option to navigate to **Screen 2**.

* Must include an option to return to the **Home screen**.

* Must access the database in some way (see Database Requirements below).

---

### **3️⃣ Screen 2**

* Must be accessible **from Screen 1** (not directly from Home).

* Must include an option to return to **Screen 1**.

* Must access the database in some way.

---

## **Required Navigation Flow (Nested Screens)**

Your screens must be nested in this order:

`Home → Screen 1 → Screen 2 → Screen 1 → Home`

You must demonstrate:

* Forward navigation (Home → 1 → 2\)

* Backward navigation (2 → 1 → Home)

* Proper screen management (no crashing, no duplicate windows left open)

Screen 2 should **not** be directly accessible from the Home screen.

---

## **Database Requirements**

Each of the following screens must interact with the database:

* Screen 1

* Screen 2

Database interaction can include:

* Running a SELECT query and displaying results

* Inserting a record

* Updating a record

* Deleting a record

* Searching/filtering records

The Home screen does not need to access the database.

---

## **Technical Expectations**

Your project should demonstrate:

* Proper use of JDBC

* Safe SQL usage (PreparedStatements)

* Closing connections/resources appropriately

* Clean navigation logic

* Functional database connection

---

## **Submission**

You will submit:

* Your code to github  
  * Make sure your database is included when you push

---

## **What Is Being Assessed**

You will be graded on:

* Correct screen nesting and navigation

* Successful database interaction on required screens

* Code organization and structure

* Stability (program runs without crashing)

* Demonstrated understanding of Lanterna window management

# **How the Internet Talks: cURL, JSON, and APIs**

## **Part 1: Beyond the Browser**

Most people use a __________________ to access websites.

But your computer can also make requests using a tool called __________________.

This lets us send requests **without** a visual interface.

---

### What is happening?

When you run a command like `curl https://github.com`, you are:

→ Sending an __________________ request
→ And receiving a __________________ in return

---

## **Part 2: Understanding Requests**

When we send a request, we can include extra information.

Match each idea:

* `-I` → Only get the __________________
* `-X POST` → Choose the __________________ of request
* `-H` → Send extra __________________ about the request
* `-d` → Send __________________ (the actual content)

---

### Think About It

Why might you want to send data instead of just requesting it?

---

## **Part 3: Data Formats (JSON)**

Websites don’t just send back pages—they send __________________.

JSON is a format used to organize __________________.

---

### JSON Basics

JSON stores data as:

→ __________ : __________ pairs

Example:

```json id="2dflks"
{
  "name": "Luke",
  "age": 19
}
```

---

### JSON can represent:

* Lists of items → __________________
* Groups of related data → __________________
* True/False values → __________________
* Text → __________________
* Numbers → __________________

---

## **Part 4: What is an API?**

An API is a way for two programs to:

→ ____________________________________________

→ ____________________________________________

---

### Real Idea

Instead of building everything yourself, you can:

→ ____________________________________________

→ ____________________________________________

---

## **Part 5: APIs as Contracts**

An API is like a __________________.

It guarantees that:

→ If you send the right __________________
→ You will get the expected __________________

---

### Why is this important?

---

---

## **Part 6: The 3 Parts of Every Request**

Every API request has three key pieces:

---

### 1. Where are you going?

This is called the __________________

Example: _______________________________________

---

### 2. What are you trying to do?

This is called the __________________

* GET → __________________ data
* POST → __________________ data
* PUT/PATCH → __________________ data
* DELETE → __________________ data

---

### 3. Extra Information

This is called the __________________

It helps the server understand things like:

→ ____________________________________________



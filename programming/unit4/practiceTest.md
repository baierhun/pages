# **Unit 4 Practice Test**

## **Multiple Choice**

**1.** What is the role of a parameter in a function?

* A. It stores the final result of a function
* B. It is a value passed into a function when it is called
* C. It defines how many times a loop runs
* D. It prints output to the screen

---

**2.** What happens when a function is called?

* A. The function is deleted
* B. The code inside the function runs
* C. The parameters are removed
* D. The program restarts

---

**3.** Which keyword is required for creating a function in Python?

* A. func
* B. define
* C. def
* D. function

---

**4.** What is the difference between a parameter and an argument?

* A. They are the same thing
* B. A parameter is used when defining a function, an argument is used when calling it
* C. A parameter is printed output
* D. An argument is inside the function header

---

**5.** Which function correctly returns the square of a number?
<table class="answer-table">
<tr><td>
* A.

```python
def square(x):
    print(x * x)
```
</td><td>
* B.

```python
def square(x):
    return x * x
```
</td></tr><tr><td>

* C.

```python
def square:
    return x * x
```
</td><td>

* D.

```python
square(x) = x * x
```
</td></tr></table>

---

## **Code Analysis**

Use the code below for Questions 6–10:

```python
1  def welcomeMessage(city):
2      print("Welcome to", city)
3      print("Have a great stay!")
4
5  def askScore():
6      score = int(input("Enter your score: "))
7      while score < 0 or score > 100:
8          print("Invalid score")
9          score = int(input("Enter your score: "))
10     return score
11
12 location = input("Where are you from? ")
13 welcomeMessage(location)
14 finalScore = askScore()
15 print(finalScore)
```

---

**6.** Which line defines a function?

* A. 1
* B. 12
* C. 13
* D. 14

---

**7.** Which lines are function calls? *(Select all that apply)*

* A. 1
* B. 13
* C. 14
* D. 6

---

**8.** Which function returns a value?

* A. welcomeMessage
* B. askScore
* C. both functions
* D. neither function

---

**9.** Which line stores the result of a function call in a variable?

* A. 12
* B. 13
* C. 14
* D. 2

---

**10.** What is the parameter in this code?

* A. score
* B. location
* C. finalScore
* D. city

---

## **Debugging & Understanding Code**

**11.** What is wrong with this code?

```python
def addNumbers(a, b):
    return a + b

result = addNumbers(4, 6, 8)
```

* A. Nothing is wrong
* B. Too many arguments are passed
* C. Missing return keyword
* D. Parameters are not defined correctly

---

**12.** What does this function output?

```python
def mystery(num):
    return num - 1

print(mystery(10))
```

* A. 11
* B. 9
* C. 10
* D. Error

---

**13.** What happens if a function has a return statement but no print statement?

* A. Nothing happens
* B. The value is automatically displayed
* C. The value is sent back to where the function was called
* D. The program crashes

---

**14.** What will this code print?

```python
def triple(x):
    return x * 3

result = triple(2)
print(result + 1)
```

* A. 6
* B. 7
* C. 8
* D. 9

---

**15.** Which statement is TRUE about function calls?

* A. Functions run only when defined
* B. Functions must always return a value
* C. Function calls execute the code inside a function
* D. Parameters are used in function calls only

---

# **Answer Key**

**1.** B  
**2.** B  
**3.** C  
**4.** B  
**5.** B  

---

**6.** A  
**7.** B, C, (D)  
**8.** B  
**9.** C  
**10.** D  

---

**11.** B  
**12.** B  
**13.** C  
**14.** B  
**15.** C  

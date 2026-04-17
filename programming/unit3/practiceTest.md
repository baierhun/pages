# **Unit 3 Practice Test – While Loops**

<style>
    .answer-table { width: 100%; border-style: hidden; margin-bottom: 60px } 
    .answer-table td { width: 50%; vertical-align: top; border: 1px solid #dfdede; padding: 10px; height: 120px; } 
    .answer-table pre { margin: 0; font-family: monospace; background-color: #496ff926} 
</style>

**1.** Which situation is **best suited** for a **count-controlled loop**?

* A. Asking the user for input until they type `"stop"`
* B. Printing numbers from 1 to 50
* C. Running until a game ends
* D. Repeating until a correct password is entered

---

**2.** Which situation is **best suited** for a **sentinel-controlled loop**?

* A. Printing numbers 1–10
* B. Looping exactly 5 times
* C. Repeating until the user enters `"exit"`
* D. Counting down from 20 to 0

---

**3.** How many times will this loop run?

```
x = 0
while x < 12:
    x += 4
```

* A. 2
* B. 3
* C. 4
* D. Infinite

---

<div class="break"></div>

**4.** What will print when this code runs?

```
x = 2
while x <= 8:
    print(x)
    x += 2
```

<table class="answer-table"><tr><td> <strong>A.</strong> <pre>2<br>4<br>6<br>8</pre> </td> <td> <strong>B.</strong> <pre>2<br>4<br>6</pre> </td> </tr> <tr> <td> <strong>C.</strong> <pre>2<br>4<br>6<br>8<br>10</pre> </td> <td> <strong>D.</strong> Infinite loop </td> </tr> </table>

---

**5.** What is wrong with this loop?

```
x = 5
while x > 0:
    print(x)
```

* A. It will run forever
* B. Syntax error
* C. Runs once
* D. Nothing is wrong

---

<div class="break"></div>

**6.** How many times will this loop run?

```
count = 1
while count < 20:
    count += 5
```

* A. 3
* B. 4
* C. 5
* D. Infinite

---

**7.** Fill in the blank so this loop prints 10, 8, 6, 4, 2:

```
x = 10
while x > 0:
    print(x)
    _____
```

* A. x += 2
* B. x -= 2
* C. x -= 1
* D. x = 2

---

**8.** What will print when this code runs?

```
x = 1
while x < 4:
    print("Hi")
    x += 1
```

<table class="answer-table"><tr><td> <strong>A.</strong> <pre>Hi<br>Hi<br>Hi</pre> </td> <td> <strong>B.</strong> <pre>Hi<br>Hi</pre> </td> </tr> <tr> <td> <strong>C.</strong> <pre>Hi<br>Hi<br>Hi<br>Hi</pre> </td> <td> <strong>D.</strong> Infinite loop </td> </tr> </table>

---

**9.** What will print when this code runs?

```
x = 6
while x > 0:
    print(x)
    x -= 3
```

<table class="answer-table"><tr><td> <strong>A.</strong> <pre>6<br>3</pre> </td> <td> <strong>B.</strong> <pre>6<br>3<br>0</pre> </td> </tr> <tr> <td> <strong>C.</strong> <pre>6<br>5<br>4<br>3<br>2<br>1</pre> </td> <td> <strong>D.</strong> Infinite loop </td> </tr> </table>

---

**10.** Which of the following best describes this loop?

```
user = input("Enter -1 to stop: ")

while user != "-1":
    print("Working...")
    user = input("Enter -1 to stop: ")
```

* A. Infinite loop
* B. Sentinel-controlled loop
* C. Count-controlled loop
* D. Nested loop

---

<div class="break"></div>

**11.** What will print when this code runs?

```
x = 0
while x < 3:
    x += 1
    print(x)
```

<table class="answer-table"><tr><td> <strong>A.</strong> <pre>0<br>1<br>2</pre> </td> <td> <strong>B.</strong> <pre>1<br>2<br>3</pre> </td> </tr> <tr> <td> <strong>C.</strong> <pre>1<br>2</pre> </td> <td> <strong>D.</strong> Infinite loop </td> </tr> </table>

---

**12.** A student is trying to write a loop that prints multiples of 3 from 3 to 15, but the code is incorrect.

```
x = 3
while x <= 15:
    print(x)
    x += 1
```

What is the **best fix**?

* A. Change `x += 1` to `x += 3`
* B. Change `x = 3` to `x = 1`
* C. Change `while x <= 15` to `while x < 15`
* D. Remove the print statement

---

<div class="break"></div>

**13.** How many times will this loop run?

```
x = 15
while x > 0:
    x -= 5
```

* A. 2
* B. 3
* C. 4
* D. Infinite

---

**14.** What will print when this code runs?

```
x = 1
while x < 5:
    print(x)
    if x == 2:
        print("Two")
    x += 1
```

<table class="answer-table"><tr><td> <strong>A.</strong> <pre>1<br>2<br>Two<br>3<br>4</pre> </td> <td> <strong>B.</strong> <pre>1<br>2<br>3<br>4<br>Two</pre> </td> </tr> <tr> <td> <strong>C.</strong> <pre>1<br>2<br>Two</pre> </td> <td> <strong>D.</strong> Infinite loop </td> </tr> </table>

---

<div class="break"></div>

**15.** What will happen with this code?

```
x = 1
while x < 5:
    print(x)
    x = x
```

* A. Prints 1 2 3 4
* B. Prints 1 forever
* C. Syntax error
* D. Prints nothing

---

### Answer Key

1. **B**
2. **C**
3. **B**
4. **A**
5. **A**
6. **B**
7. **B**
8. **A**
9. **A**
10. **B**
11. **B**
12. **A**
13. **B**
14. **A**
15. **B**

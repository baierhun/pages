# Strings in Java – Practice Worksheet

**Name:** ____________________________________
**Date:** ____________________________________

## Part 1: String Basics

**Fill in the blank or answer the question.**

1. In Java, __________________________ are objects that hold sequences of characters.

2. Class names begin with a __________________ letter, while primitive types begin with a __________________ letter.

3. A __________________________ is a set of characters enclosed in double quotes (`"`).

4. Strings can be appended to each other with the `+` or `+=` operators. This is called __________________________.

5. What is the difference between a **String** and a **char**?

---

---

6. Write a String variable named `firstName` that stores the value `"Charles"`.

```java


```

7. Write a String variable named `favoriteFood` that stores your favorite food.

```java


```

---

## Part 2: Is the Code Valid?

**For each code segment, write V if the code is valid or I if the code is invalid. If it is invalid, explain what is wrong.**

8. `String value = 1234;`

**V / I:** __________

If invalid, what is wrong?

---

9. `String letter = A;`

**V / I:** __________

If invalid, what is wrong?

---

<div class="break"></div>

10. `String let = "A";`

**V / I:** __________

If invalid, what is wrong?

---

11. `String firstName = new String("Charles");`

**V / I:** __________

If invalid, what is wrong?

---

12. `String name = new String(Bob);`

**V / I:** __________

If invalid, what is wrong?

---

13. `"Bob" = String name;`

**V / I:** __________

If invalid, what is wrong?

---

14. `String phoneNumber = "(555) 888-1212";`

**V / I:** __________

If invalid, what is wrong?

---

15. `String book = "I like "Harry Potter"";`

**V / I:** __________

If invalid, how could you fix it?

```java


```

---

<div class="break"></div>

## Part 3: String Concatenation

Consider the following code:

```java
String name1 = "Bob";
String name2 = "The Builder";
```

16. Write a line of code that creates a variable named `fullName` containing `name2` followed by `name1`.

```java


```

17. What value will be stored in `fullName`?

---

18. Write a line of code that creates a variable named `description` containing:

`"3 Little Pigs!"`

Use the variables below:

```java
String animal = "Pigs";
String descriptor = "Little";
```

```java


```

19. What value will be stored in `description`?

---

---

## Part 4: Working with String Variables

Consider the following code:

```java
String thing1 = "Cat in";
String thing2 = "the";
String phrase = thing1 + " " + thing2 + " Hat";
```

20. What value is stored in `phrase`?

---

<div class="break"></div>

21. Write code that creates a new String variable named `sentence` containing:

`I like "Cat in the Hat"!`

```java


```

22. What value is stored in `sentence`?

---

23. Write code that creates a new String variable named `reversed` containing `thing2`, two spaces, and then `thing1`.

```java


```

24. What value is stored in `reversed`?

---

---

## Part 5: Predict the Value of a Variable

**For each question, write the value that will be stored in the variable.**

25.

```java
String word1 = "Hello";
String word2 = "World";
String result = word1 + word2;
```

**Value of `result`:** __________________________________________

26.

```java
String word1 = "Hello";
String word2 = "World";
String result = word1 + " " + word2;
```

**Value of `result`:** __________________________________________

27.

```java
String animal = "dog";
String result = "My " + animal + " is happy.";
```

**Value of `result`:** __________________________________________

28.

```java
String first = "AP";
String second = "Computer";
String third = "Science";
String result = first + " " + second + " " + third;
```

**Value of `result`:** __________________________________________

29.

```java
String message = "Score: ";
message += "100";
```

**Value of `message`:** __________________________________________

---

## Part 6: Write the Code

30. Create a String variable named `school` that stores the name of your school.

```java


```

31. Create a String variable named `greeting` that stores:

`Hello, [your name]!`

```java


```

32. Given:

```java
String firstName = "John";
String lastName = "Smith";
```

Write code that creates a variable named `fullName` containing:

`John Smith`

```java


```

<div class="break"></div>

33. Given:

```java
String item = "pizza";
String adjective = "delicious";
```

Write code that creates a variable named `sentence` containing:

`The pizza is delicious!`

```java


```

34. Given:

```java
String number = "42";
```

Write code that creates a variable named `message` containing:

`The answer is 42.`

```java


```

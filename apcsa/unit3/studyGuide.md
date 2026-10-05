<div class="title">
    <h1>
        AP Computer Science A
    </h1>
    <div class="print-on">
        <strong>Name:</strong>&nbsp;<span>&nbsp;</span>
    </div>
</div>

## Unit 3 Interactive Study Guide

---

## Strings

### String Basics

A `String` is a sequence of ______________________________.

The `length()` method returns the number of ______________________________ in a String.

Example:

```java
String word = "Computer";
int x = word.length();
```

The value of `x` is __________________.

A **method** is a block of code that ______________________________ a specific task.

When we call a method, the information we put inside the parentheses is called an ______________________________.

The value that a method sends back is called the ______________________________ value.

### `charAt()`

The `charAt()` method returns the ______________________________ at a specified index.

The index of the first character in a String is __________________.

```java
String word = "Computer";
char letter = word.charAt(2);
```

The value of `letter` is __________________.

The argument passed to `charAt()` represents the character's ______________________________.

---

## More String Methods

Complete the table.

| Method                  | What does it do?                                                           |
| ----------------------- | -------------------------------------------------------------------------- |
| `length()`              | Returns the number of ______________________________                       |
| `charAt(index)`         | Returns the ______________________________ at an index                     |
| `substring(start, end)` | Returns part of a ______________________________                           |
| `indexOf(str)`          | Returns the ______________________________ where a String is found         |
| `equals(str)`           | Checks whether two Strings contain the same ______________________________ |
| `compareTo(str)`        | Compares two Strings ______________________________                        |
| `toUpperCase()`         | Converts letters to ______________________________                         |
| `toLowerCase()`         | Converts letters to ______________________________                         |

### String Indexes

Consider:

```java
String word = "Hello";
```

| Character | H     | e     | l     | l     | o     |
| --------- | ----- | ----- | ----- | ----- | ----- |
| Index     | _____ | _____ | _____ | _____ | _____ |

The last valid index is always ______________________________ than the String's length.

### `substring()`

```java
String word = "Computer";
String part = word.substring(1, 4);
```

The value of `part` is ______________________________.

The first argument tells Java where to ______________________________.

The second argument tells Java where to ______________________________ (but that index is not included).

### `indexOf()`

```java
String word = "Computer";
int x = word.indexOf("put");
```

The value of `x` is __________________.

If `indexOf()` cannot find the requested String, it returns __________________.

### `equals()`

To compare the contents of two Strings, we should use ______________________________ rather than `==`.

```java
String a = "hello";
String b = "hello";

a.equals(b)
```

This expression evaluates to __________________.

### `compareTo()`

`compareTo()` returns a negative number when the first String comes ______________________________ the second String alphabetically.

It returns `0` when the two Strings are ______________________________.

It returns a positive number when the first String comes ______________________________ the second String alphabetically.

### String Exceptions

A `StringIndexOutOfBoundsException` occurs when we try to access a String using an ______________________________ index.

For example:

```java
String word = "Hello";
char x = word.charAt(10);
```

This causes a `________________________________________`.

---

## Custom Class Methods

### Public vs. Private

A `public` method can be accessed ______________________________ a class.

A `private` method can only be accessed ______________________________ the class where it is defined.

The keyword used to make a method accessible from outside the class is ______________________________.

The keyword used to restrict a method to the class itself is ______________________________.

### Preconditions and Postconditions

A **precondition** describes what must be ______________________________ before a method is called.

A **postcondition** describes what will be ______________________________ after the method runs.

For example:

```java
/**
 * Precondition: amount is greater than 0
 * Postcondition: the balance increases by amount
 */
public void deposit(double amount)
```

The precondition is that `amount` must be ______________________________.

The postcondition is that the ______________________________ increases.

---

## Custom Class Methods — Review and `static`

A method that belongs to a particular object is called an ______________________________ method.

An instance method is called using an ______________________________.

A `static` method belongs to the ______________________________ rather than to a particular object.

A static method can be called using the ______________________________ name.

For example:

```java
Math.random();
```

`random()` is a ______________________________ method.

### `NullPointerException`

A reference variable can contain the special value ______________________________.

`null` means that the reference does not currently refer to a ______________________________.

Consider:

```java
Student s = null;
s.getName();
```

This causes a `________________________________________`.

A `NullPointerException` occurs when we try to use a reference that contains ______________________________.

---

## 20. Memory and Variable Scope

### Stack and Heap

Local variables and method parameters are stored in the ______________________________.

Objects created with `new` are stored in the ______________________________.

Primitive variables store their actual ______________________________.

Reference variables store a ______________________________ to an object.

Instance variables are part of an ______________________________ and are stored with that object on the heap.

### Primitive vs. Reference

Consider:

```java
int x = 10;
Student s = new Student();
```

`x` is a ______________________________ variable.

`s` is a ______________________________ variable.

The value stored in `x` is ______________________________.

The value stored in `s` is a ______________________________ to an object.

### Scope

The **scope** of a variable is the part of the program where that variable can be ______________________________.

A local variable declared inside a method can generally only be accessed ______________________________ that method.

An instance variable belongs to an ______________________________ and can be accessed by the object's methods.

### References and `null`

Consider:

```java
Student s = null;
```

`s` is a ______________________________ variable.

The value of `s` is ______________________________.

At this point, `s` does not refer to an actual ______________________________.

If we write:

```java
s.getName();
```

Java throws a `________________________________________`.

### Exceptions Review

Complete each statement.

A `StringIndexOutOfBoundsException` is usually caused by an invalid String ______________________________.

A `NullPointerException` is usually caused by attempting to use an object ______________________________.

An exception is a problem that occurs while a program is ______________________________.

---

## Math and Integer Libraries

Java provides useful classes containing methods we can use in our programs.

The `Math` class provides methods for ______________________________ and mathematical operations.

The `Integer` class provides methods for working with ______________________________ values.

### Math Methods

Complete the descriptions.

| Method           | What does it do?                                                                                |
| ---------------- | ----------------------------------------------------------------------------------------------- |
| `Math.abs(x)`    | Returns the ______________________________ value                                                |
| `Math.pow(x, y)` | Raises `x` to the power of __________________                                                   |
| `Math.sqrt(x)`   | Returns the ______________________________ of `x`                                               |
| `Math.max(x, y)` | Returns the ______________________________ value                                                |
| `Math.min(x, y)` | Returns the ______________________________ value                                                |
| `Math.random()`  | Returns a random `double` from ______________________________ to ______________________________ |

Most methods in the `Math` class are called using the class name because they are ______________________________ methods.

### Integer Methods

`Integer.parseInt()` converts a String into an ______________________________.

```java
String s = "42";
int x = Integer.parseInt(s);
```

The value of `x` is __________________.

`Integer.parseDouble()` belongs to the ______________________________ class.

True or False:

`Integer.parseInt("hello")` can successfully convert `"hello"` into an integer.

**Answer:** __________________

---

# Final Review

Fill in each blank with the most important term.

1. A String is a sequence of ______________________________.

2. The first String index is __________________.

3. `length()` returns the number of ______________________________.

4. `charAt()` returns a ______________________________.

5. `substring()` returns part of a ______________________________.

6. `equals()` compares the ______________________________ of Strings.

7. An invalid String index can cause a ______________________________.

8. A method that belongs to a class rather than an object is ______________________________.

9. A reference that does not refer to an object contains ______________________________.

10. Trying to use a `null` reference can cause a ______________________________.

11. Primitive values are stored directly in a variable, while reference variables store a ______________________________ to an object.

12. Objects created with `new` are stored on the ______________________________.

13. Local variables and parameters are stored on the ______________________________.

14. A precondition tells us what must be true ______________________________ a method runs.

15. A postcondition tells us what is true ______________________________ a method runs.

16. `Math.random()` is a ______________________________ method.

17. `Integer.parseInt()` converts a String into an ______________________________.

18. The scope of a variable is where that variable can be ______________________________.

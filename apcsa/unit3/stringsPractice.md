# Strings Practice

Complete the following scenarios in problem set 3. Use a new file for each scenario.

### 🔐 1. Secret Code Breaker

Create a program using:

```java
String code = "X7BLUE42CAT9";
```

* Find and store the length of the code.
* Extract `"BLUE"` and store it in a String variable.
* Extract `"CAT"` and store it in a String variable.
* Find and store the position where `"42"` begins.

---

### 🕵️ 2. What's My Username?

Create a program using:

```java
String email = "steve.jobs@apple.com";
```

* Find the position of the `@`.
* Extract the username (`"steve.jobs"`).
* Extract the domain (`"apple.com"`).
* Change the email to a different email address and make sure your code still works.

---

### 🧩 3. Word Detective

Create a program using:

```java
String word1 = "elephant";
String word2 = "elephantine";
```

* Determine whether the two words are exactly equal.
* Find the length of each word.
* Compare the two words alphabetically.
* Determine which word comes first alphabetically.

---

<div class="break"></div>

### 🎮 4. Character Name Generator

Create a program using:

```java
String name = "Taylor Swift";
```

* Find the position of the space.
* Extract the first name.
* Extract the last name.
* Create a username using the first name, a period, and the last name.
* Create another username using the first letter of the first name followed by the last name.

Example:

```text
tSwift
```

---

### 🏆 5. High Score Leaderboard

Create a program using:

```java
String player1 = "Mario";
String player2 = "Luigi";
```

* Compare the two player names alphabetically.
* Determine which player should appear first on an alphabetical leaderboard.
* Store your result in a `boolean` variable.
* Change the player names and make sure your code still works.

---

<div class="break"></div>

### 🔑 6. Password Validator

Create a program using:

```java
String password = "Tiger2026!";
```

Check the password for the following:

* The password is at least 8 characters long.
* The password contains `"2026"`.
* The password contains `"!"`.
* The password is not exactly `"password"`.

Store each result in a variable. Then create a final `boolean` variable that determines whether the password passes all of the requirements.

---

### 🕵️ 7. Hidden Message

Create a program using:

```java
String message = "The secret word is BANANA. Do not tell anyone.";
```

* Find the position where `"BANANA"` begins.
* Extract the secret word.
* Find the length of the secret word.
* Create a `String` variable called `guess` containing `"BANANA"`.
* Determine whether the guess is correct.

---

### 🏴‍☠️ 8. Pirate Treasure Map

Create a program using:

```java
String map = "NORTH-EAST-TREASURE-CAVE";
```

Extract each piece of information from the map:

* `"NORTH"`
* `"EAST"`
* `"TREASURE"`
* `"CAVE"`

Use `indexOf()` and `substring()` to find the locations of the different pieces rather than hard-coding the positions.

---

### 🤖 9. Chatbot Response

Create a program using:

```java
String message = "I want to order pizza";
```

* Determine whether the message contains `"pizza"`.
* Determine whether the message contains `"burger"`.
* Create a `boolean` that determines whether the message contains either `"pizza"` or `"burger"`.
* Test your program with several different messages.

Try:

```text
I want pizza
Do you have burgers?
I would like a salad
What time do you close?
```

---

### 🎬 10. Movie Rating Challenge

Create a program using:

```java
String movie1 = "Avatar";
String movie2 = "Avengers";
```

* Extract the first three characters of each movie title.
* Determine whether the first three characters are equal.
* Compare the complete movie titles alphabetically.
* Determine which movie comes first alphabetically.
* Test your program with different movie titles.

---

<div class="break"></div>

### 🔓 11. Final Lock

Create a program using:

```java
String clue = "TREASURE:DRAGON:CAVE";
```

Use String methods to extract:

* `"TREASURE"`
* `"DRAGON"`
* `"CAVE"`

Then create three variables containing a player's answers.

Determine whether **all three answers are correct**.

Finally, change the clue to:

```java
String clue = "CASTLE:WIZARD:FOREST";
```

Your program should still work without changing the code that finds the different pieces.

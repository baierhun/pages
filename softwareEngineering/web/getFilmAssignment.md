# **Assignment: Planet Details Page (SWAPI + Lanterna)**

## **Objective**

Extend your Star Wars terminal app by adding a new page that displays detailed information about a planet.

Users should be able to:

1. Click on a planet from a person’s detail page
2. Navigate to a new **Planet page**
3. View detailed information about that planet

---

## **What You Already Have**

* A **People list page** (from `/people`)
* A **Person detail page**
* The ability to:

  * Make API calls to SWAPI
  * Display a person’s **homeworld (planet)**
  * Fetch planet data using the planet URL

---

## **Your Task**

### **1. Create a New Window**

Create a new class:

```
ui/windows/PlanetWindow.java
```

This window will display all planet-related information.

---

### **2. Add Navigation**

From your **PersonWindow**:

* Make the **planet name clickable**
* When clicked:

  * Open your new `PlanetWindow`
  * Pass in the planet URL

---

### **3. Fetch Planet Data**

Use the planet URL to make an API request.

From the response, you will need:

* `name`
* `residents` (list of URLs)
* `films` (list of URLs)

---

### **4. Display Planet Information**

Your `PlanetWindow` must show:

#### ✅ Planet Name

```
Tatooine
```

#### ✅ Number of Characters From This Planet

* Use the `residents` array
* Display the **count only**

Example:

```
Residents: 10
```

---

### **5. Fetch Film Names (Important Part 🚀)**

The `films` field contains URLs like:

```
https://swapi.dev/api/films/1/
```

You must:

1. Loop through each film URL
2. Make an API call for each one
3. Extract the **film title**

---

### **6. Display Film Names**

Example output:

```
Films:
- A New Hope
- Return of the Jedi
- The Phantom Menace
```

---

## **Requirements Checklist**

* [ ] Create `PlanetWindow`
* [ ] Navigate to it from `PersonWindow`
* [ ] Fetch planet data using API
* [ ] Display planet name
* [ ] Display number of residents
* [ ] Make additional API calls for films
* [ ] Display all film names in a list

---

## **Hints (Don’t Skip These)**

* You already solved this once with:

  * Person → Planet
    Now you're doing:
  * Planet → Films

* Think about reusing:

  * Your API helper methods
  * Your JSON parsing logic

* Film requests will likely require:

```java
for (String filmUrl : films) {
    // make API call
}
```

---

## **Submission**

* Push your updated project to GitHub
* Make sure navigation works end-to-end:

  * People → Person → Planet


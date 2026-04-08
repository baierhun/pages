# 🟡 Assignment: Star Wars App – Enhancements

You’ve already explored an app using Lanterna that fetches Star Wars characters from the SWAPI. Now it’s time to improve performance and add deeper functionality.

---

## 🎯 Objective

Enhance your application by:

* Reducing lag with caching
* Adding a detailed view for each character
* Fetching related data (planet names instead of URLs)

---

## ✅ Tasks

### **1. Add Basic Caching (Performance Improvement)**

Right now, your app makes repeated API calls, which causes lag.

**Your task:**

* Add a simple in-memory cache to store API responses

**Requirements:**

* Cache results from API calls (e.g., people, planets)
* If data has already been fetched, return it from the cache instead of calling the API again
* You can simply store the data in an instance variable.

**Goal:**
Your app should feel noticeably faster when reopening data.

---

### **2. Create a Person Detail Page**

We want to view more information about a character when selected.

#### 🔧 Create a New Window

* File name: `PersonWindow`
* Location: `ui/windows`

#### 🖥 Display the Following:

* Name
* Homeworld (for now, this will still be a URL)
* Birth year

#### 🔗 Add Navigation

* When the user selects (clicks) a character from the list:

  * Open the `PersonWindow`
  * Pass the selected `Person` into the window

**Hint:**
You’ll likely modify your existing list UI to add a click handler or selection listener.

---

### **3. Replace Planet URL with Planet Name**

Right now, you're displaying a URL for the homeworld. Let’s fix that.

#### 🔧 Step 1: Create a `Planet` Record

Create a new record to represent a planet.

Include all fields from the planet endpoint

---

#### 🔧 Step 2: Create `PlanetService`

Create a new service class to fetch planet data.

**Requirements:**

* Method: `getPlanet`
* This method should:

  * Make an API call to the given URL
  * Parse the response
  * Return a `Planet`

---

#### 🔧 Step 3: Use the Service in `PersonWindow`

* Add `PlanetService` to your `PersonWindow`
* Use the person’s homeworld URL to:

  * Fetch the planet
  * Display the **planet’s name** instead of the URL

---

### 💡 Final Result

When your app is complete:

* Selecting a character opens a new window with details
* The homeworld displays a **planet name**, not a URL
* The app runs faster due to caching

---
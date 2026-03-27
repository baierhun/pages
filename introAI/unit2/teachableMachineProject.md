## **Final Project: Build a Purpose-Driven Teachable Machine (with Multiple Classes)**

### **Objective**

You will design, train, test, and iterate a machine learning model that performs a **practical task**, classifies inputs into **at least 3 categories**, and demonstrates improvement through multiple iterations. The model should be **robust enough to work reliably in different real-world settings**.

---

### **Step 1: Define a Purpose**

* Identify a **real-world problem or useful task** for the model.
* Examples:

  * **Classroom helper:** Detect hand raised / hand lowered / empty desk
  * **Health & safety:** Mask / no mask / incorrect mask
  * **Daily life convenience:** Recycling / compost / trash

> **Requirement:** The model must have **at least 3 classes**.

---

### **Step 2: Collect & Prepare Data**

* Gather examples for each class. **Minimum numbers depend on the data source:**

  * **Webcam capture:** Minimum 800 images per class
  * **Uploaded images from files:** Minimum 100 images per class
* Include **variation**: angles, lighting, background, multiple people, and different environments if possible
* Document each sample (date, conditions, label)

---

### **Step 3: Train the Model**

* Use [Teachable Machine](https://teachablemachine.withgoogle.com/)
* **Train multiple times**, experimenting with:

  * Number of examples per class
  * Category definitions
* Track changes in accuracy after each iteration

---

### **Step 4: Test & Iterate**

* Test with **new, unseen examples** for each class
* Test in **different settings** (lighting, background, angles) to ensure robustness
* Record:

  * Misclassifications
  * Accuracy per class
  * Overall accuracy
* Iterate by adjusting:

  * Adding more samples
  * Refining categories
  * Retraining the model

> **Minimum requirement:** You must do **at least 2 iterations** and show measurable improvement.

> **Key requirement:** Models must **perform reliably in settings outside of where they were trained**.

---

### **Step 5: Demonstrate Practical Use**

* Live demos in class
* Show how the model performs its **intended function** reliably

---

### **Step 6: Download & Submit**

* Download the trained project as a **`.tm` file**
* Submit the `.tm` file to **Canvas** for grading

> This allows the instructor to open the model and verify its functionality in **different settings**.

---

### **Step 7: Reflection & Presentation**

Present:

1. **Problem & purpose** – why they built this model
2. **Classes & data** – what the classes are, how they collected samples
3. **Iterations & testing** – what they changed and why
4. **Results** – accuracy, reliability, and usability
5. **Lessons learned** – challenges, misclassifications, and improvements

---

### **Evaluation / Rubric**

* **Purpose & Relevance:** Useful task? At least 3 classes?
* **Data & Iteration:** Sufficient examples per source, multiple iterations
* **Performance / Robustness:** Model works reliably **in different real-world settings**
* **Presentation:** Clear live demonstration & explanation
* **Submission:** Correct `.tm` file submitted to Canvas
* **Creativity & Innovation:** Unique approach or solution


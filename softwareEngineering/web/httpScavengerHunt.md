## 🕵️‍♂️ 5-Minute Network Scavenger Hunt
**Setup:** Open **Inspect** (F12) > **Network** tab. Refresh the page!

1.  **The "Postman":** Find a request where the **Method** is **POST**. 
    * *Hint: Try clicking a "Like" button, a "Login" button, or submitting a form.*
2.  **The "Question":** Find a URL containing a **`?`** (Query Parameter).
    * *Click the request and check the **Payload** tab. What is one "Key" and "Value" you see?*
3.  **The "Redirection":** Find a **301** or **302** Status Code.
    * *This means the server is pointing you to a different URL!*
4.  **The "Not Okay":** Find a Status Code that is **NOT** `200`. 
    * *Can you find a `304` (Cached/Not Modified) or a `204` (No Content)?*
5.  **The "Identity":** Find a request where the **Method** is **OPTIONS** or **PUT**.
    * *Hint: These are often used by APIs to check permissions or update data.*

---

### 💡 Quick Cheat Sheet:
* **200:** OK (Success!)
* **204:** No Content (Success, but nothing to show)
* **304:** Not Modified (Using the version saved in your browser cache)
* **404:** Not Found (That URL doesn't exist)
* **POST:** Sending data *to* the server.
* **GET:** Asking for data *from* the server.
{expand:title=🧩 Chapter 3: Functions}
*h2. 🔑 Key Takeaway*  
Functions should be small, do *one thing*, and do it *well*. They are the building blocks of clean, understandable code.

---

*h3. ✅ Key Principles of Clean Functions*

# *Small in size*  
  - Functions should be 2–4 lines whenever possible.
  - If it’s over 20 lines, consider breaking it.

# *Do one thing only*  
  - A function should do one task and do it completely.
  - If you can extract part of it and describe it with another verb, it does more than one thing.

# *Use descriptive names*  
  - Function names should clearly describe *what* they do.
  - Use verbs for commands (e.g., `calculateTotal()`, `fetchOrders()`).

# *Use fewer arguments*  
  - Ideal: 0–2 arguments
  - Avoid flag arguments (e.g., `isSorted = true`) — it means the function does more than one thing.

# *Avoid side effects*  
  - Functions should not alter global state or input objects unless that's the primary purpose.
  - Pure functions are easier to test and reason about.

# *Use command-query separation*  
  - A function should either do something (command) *or* return something (query) — not both.

# *Structured for readability*  
  - Use meaningful white space and separation of concerns.
  - The top-down narrative should be readable like prose.

---

*h3. 🧪 Examples*

*❌ Bad:*
{code:java}
public void processUserData(User user) {
    validateUser(user);
    saveUser(user);
    sendWelcomeEmail(user);
}
{code}

This function does *more than one thing*: validation, persistence, and notification.

*✅ Good:*
{code:java}
public void onboardNewUser(User user) {
    if (isValid(user)) {
        registerUser(user);
        notifyUser(user);
    }
}
{code}

---

*h3. 📌 Function Design Checklist*

|| Principle                   || Recommendation                       ||
| Small Size                  | Max 2–4 lines if possible             |
| Do One Thing                | One clear purpose                     |
| Good Name                   | Verb-based, descriptive               |
| Few Arguments               | 0–2 preferred                         |
| No Side Effects             | Especially hidden/global              |
| Clear Structure             | Top-down readability                  |

---

*bq. “Functions should do something, or answer something, but not both.”*  
— *Robert C. Martin*

{expand}

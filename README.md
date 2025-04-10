h2. 🏷️ Chapter 2: Meaningful Names

*h3. 🔑 Key Takeaway*  
Good naming is fundamental to writing clean code. Names should reveal *intent*, be *unambiguous*, and help readers *understand the system* without extra explanation.

---

*h3. ✅ What Makes a Name “Meaningful”?*

# *Reveals intent*  
A name should clearly express what the variable, function, or class is for.
{code:java}
    // Bad
    int d; // what is 'd'?

    // Good
    int elapsedTimeInDays;
{code}

# *Avoids disinformation*  
Avoid misleading names or names that mean something else in programming.  
Don’t name a collection 'accountList' if it’s actually a Set.

# *Makes code searchable*  
Avoid single-letter variables like x or q. Prefer 'customerAddress' over 'addr'.

# *Is pronounceable*  
{code:java}
    // Bad
    String genymdhms;

    // Good
    String generationTimestamp;
{code}

# *Follows conventions*  
* Classes: Nouns (e.g., *OrderProcessor*, *UserProfile*)  
* Methods: Verbs (e.g., *saveUser()*, *calculateTax()*)

# *Avoids encodings*  
No need for prefixes like *m_*, *i_*, or Hungarian notation in modern IDEs.

# *Avoids noise words*  
Words like *data*, *object*, or *info* don’t add value.  
Prefer *address* over *addressInfo* or *addressData*.

---

*h3. 🧪 Real-World Example*

*❌ Poor Naming:*
{code:java}
public void getData() {
    // does what?
}
{code}

*✅ Better Naming:*
{code:java}
public List<Customer> fetchActiveCustomers() {
    // clearly explains what is returned
}
{code}

---

*h3. 🧼 Naming Tips Summary*

|| Principle               || Example                         ||
| Reveal intent            | startDate vs d                   |
| Be specific              | getActiveUsers() not getData()   |
| Avoid mental mapping     | customer not cust                |
| Use domain terms         | Portfolio, Transaction           |
| Be consistent            | get, set, fetch, calculate       |

---

*bq. “The name of a variable, function, or class should answer all the big questions. It should tell you why it exists, what it does, and how it is used.”*  
— *Robert C. Martin*

{expand:title=💬 Chapter 4: Comments}
*h2. 🔑 Key Takeaway*  
The best code needs no comments. Comments are a *failure to express intent through code itself*. Use them only when necessary, and never to excuse bad code.

---

*h3. 🚫 Most Comments Are Bad*

- Comments are often used as a crutch for unclear code.
- They rot easily — becoming outdated and misleading.
- Clean code should be *self-explanatory* without comments.

---

*h3. ✅ When Comments Are Acceptable*

# *Legal or Licensing Information*  
Required by law or company policy.

# *Clarifying Intent (when code cannot express it well)*  
{code:java}
// Use binary search for optimal performance with large arrays
int index = binarySearch(data, target);
{code}

# *Warning of Consequences*  
{code:java}
// Do not delete before archiving — critical audit trail
archive(transaction);
{code}

# *TODOs (temporary but visible notes)*  
{code:java}
// TODO: Replace this with an async retry mechanism
{code}

---

*h3. 🚫 Examples of Bad Comments*

# *Redundant Comments*  
{code:java}
// increment i
i++; 
{code}

# *Misleading or Outdated Comments*  
{code:java}
// set timeout to 5 seconds
setTimeout(3000); // actually 3 seconds
{code}

# *Noise Comments*  
{code:java}
// Check if user is null
if (user != null) {
    ...
}
{code}

---

*h3. 🧼 Best Practice: Code Should Explain Itself*

Instead of this:
{code:java}
// Check if employee is eligible for bonus
if (employee.getTenure() > 5 && employee.getPerformanceRating() > 4) {
{code}

Write this:
{code:java}
if (employee.isEligibleForBonus()) {
{code}

---

*h3. 🧪 Comment Guideline Summary*

|| Type of Comment       || Good? || Notes                              ||
| Legal / License        | ✅     | Required in most projects           |
| Explanation of Intent  | ✅     | When code alone isn't enough        |
| Warning of Side Effects| ✅     | Critical operations                 |
| TODOs                  | ✅     | Temporary with follow-up            |
| Redundant / Obvious    | ❌     | Avoid                              |
| Outdated or Wrong      | ❌     | Dangerous, must be removed          |

---

*bq. “Don’t use a comment when you can make the code self-explanatory.”*  
— *Robert C. Martin*

{expand}

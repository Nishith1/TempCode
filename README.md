h1. 🧼 Clean Code – Chapter Summaries

Below are summaries of chapters from the book *Clean Code* by Robert C. Martin. Expand each chapter to read more.

{expand:title=📘 Chapter 1: Clean Code}
*h2. 🔑 Key Takeaway*  
Clean code is readable, maintainable, and shows the care of the developer.

*h3. Quotes:*  
- “Clean code is simple and direct.” — Grady Booch  
- “Looks like it was written by someone who cares.” — Michael Feathers  
- “Elegant and efficient.” — Bjarne Stroustrup

*h3. Characteristics:*  
- Minimal duplication  
- Clear structure  
- Small functions  
- Self-documenting names  
- Well-tested

*bq. “You know you are working with clean code when each routine you read turns out to be pretty much what you expected.”*
{expand}

{expand:title=🏷️ Chapter 2: Meaningful Names}
*h2. 🔑 Key Takeaway*  
Names should clearly reveal the intent and help in understanding the code without extra comments.

*h3. Good Naming Principles:*
# Reveals intent  
# Avoids disinformation  
# Is searchable  
# Is pronounceable  
# Follows conventions  
# Avoids noise words

*Example:*
{code:java}
// Bad
int d;

// Good
int elapsedTimeInDays;
{code}

*Real-World Function Example:*
{code:java}
// Poor
public void getData() {}

// Better
public List<Customer> fetchActiveCustomers() {}
{code}

*Summary Table:*
|| Principle               || Example                         ||
| Reveal intent            | startDate vs d                   |
| Be specific              | getActiveUsers() not getData()   |
| Avoid mental mapping     | customer not cust                |
| Use domain terms         | Portfolio, Transaction           |
| Be consistent            | get, set, fetch, calculate       |

*bq. “The name of a variable, function, or class should answer all the big questions. It should tell you why it exists, what it does, and how it is used.”*
{expand}

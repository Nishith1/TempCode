{expand:title=📐 Chapter 5: Formatting}
*h2. 🔑 Key Takeaway*  
Code formatting is about communication. Well-formatted code is easier to read, understand, and maintain — it expresses structure and intent clearly.

---

*h3. 🧭 Why Formatting Matters*

- Developers read code more often than they write it.
- Consistent formatting allows readers to grasp structure and flow quickly.
- Code is a form of written communication, not just instruction to machines.

---

*h3. 📐 Vertical Formatting*

# *Small files are better*  
  - Limit files to 200–500 lines if possible.
  - Each file should represent a cohesive concept.

# *Vertical density*  
  - Group related code blocks together.
  - Use blank lines to separate logical sections.

# *Ordering of functions*  
  - Organize from high-level to low-level (top-down narrative).
  - Functions called higher in the call stack appear above helpers.

---

*h3. ↔️ Horizontal Formatting*

# *Line length*  
  - Limit lines to ~100–120 characters.
  - Break long expressions into smaller ones.

# *Consistent indentation*  
  - Indentation must reflect block structure.
  - Avoid deep nesting by extracting functions.

# *Spaces matter*  
  - Use spacing to aid clarity:
{code:java}
// Better
if (user.isActive()) {
    sendEmail(user);
}
// Worse
if(user.isActive()){sendEmail(user);}
{code}

---

*h3. 📦 Code Blocks and Indentation*

- Each block enclosed in `{}` should be properly indented.
- Keep nesting shallow — no more than 2-3 levels.
- Use early returns to reduce nested `if-else` blocks.

---

*h3. 🧪 Formatting Example*

*❌ Poor Formatting:*
{code:java}
public void process(){if(user!=null){if(user.isActive()){sendEmail(user);}}}
{code}

*✅ Clean Formatting:*
{code:java}
public void process() {
    if (user == null) return;

    if (user.isActive()) {
        sendEmail(user);
    }
}
{code}

---

*h3. 📌 Formatting Best Practices*

|| Guideline                  || Recommendation                    ||
| File length                 | ~200–500 lines                    |
| Function order              | High-level first                  |
| Blank lines                 | Use to separate logic sections    |
| Max line length             | 100–120 characters                |
| Indentation                 | Consistent and meaningful         |
| Nesting depth               | Keep shallow (≤2–3 levels)        |
| Vertical openness/density  | Structure should "breathe"        |

---

*bq. “You should take care that the formatting of your code maximizes its readability.”*  
— *Robert C. Martin*

{expand}

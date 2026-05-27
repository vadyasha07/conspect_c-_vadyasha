_**Chapter 7(Scope, Duration, and Linkage)**
---

(Linkage)
static or anonymous namespace — hides a function/variable within the file (Internal). Use this to avoid name conflicts.

extern — indicates that the variable is defined in another file. Do not initialize it in main.cpp using parentheses!

inline (constexpr) — global constants in .h files (Best Practice). - We tell the compiler that in all files where a variable with the same name as in the .h file is included, it should simply be replaced with the contents of that file, without any crashes or errors

---
**!!! Avoid using static variables inside functions to maintain state if that state can be explicitly passed via arguments. !!!**
---

**Best practice**
Const static local variables are generally okay to use.

Non-const static local variables should generally be avoided. If you do use them, ensure the variable never needs to be reset, and isn’t used to alter program flow.

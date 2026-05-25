Chapter 7(Scope, Duration, and Linkage)

(Linkage)
static or anonymous namespace — hides a function/variable within the file (Internal). Use this to avoid name conflicts.

extern — indicates that the variable is defined in another file. Do not initialize it in main.cpp using parentheses!

inline (constexpr) — global constants in .h files (Best Practice).

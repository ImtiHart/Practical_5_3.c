# Character Occurrence Finder (C)

A C program that searches a fixed paragraph for every occurrence of a user-supplied
character, printing each match's **position**, **pointer address**, and a **total count** —
using `strchr()` in a loop.

## 🎯 What It Demonstrates

- **`strchr()` iteration** — the idiomatic C pattern of repeatedly calling `strchr`
  and advancing the cursor past each match (`ptr++`), stopping at `NULL`.
- **Pointer arithmetic** — `ptr - base` yields the character's index; `%p` prints
  the raw memory address.
- **Defensive coding** — `NULL` checks prevent dereferencing past the end of the
  string, and a "not found" message handles the zero-match case.

## 🚀 How to Run

```bash
gcc main.c -o finder
./finder

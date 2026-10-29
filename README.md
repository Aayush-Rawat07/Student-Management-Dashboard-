# Student Grade Management System

A feature-rich, console-based **Grade Management System** written in **C**, demonstrating core and advanced C programming concepts including recursive algorithms, dynamic memory allocation, and file persistence.

---

## Features

| Feature | Details |
|---|---|
| **Add Student** | Name, roll number (unique, validated), marks per subject |
| **View Students** | Formatted card layout with rank, grade, percentage |
| **Update Student** | Edit name, roll number, and marks with full validation |
| **Delete Student** | With confirmation prompt before deletion |
| **Search** | By roll number (Recursive Binary Search) or name (Recursive Linear Search) |
| **Sort** | By total marks descending or roll number ascending (Recursive QuickSort) |
| **Class Statistics** | Average, top/low scorer, pass/fail count, grade distribution |
| **Subject Analysis** | Per-subject class average, highest, and lowest scorer |
| **Save / Load** | Binary file persistence (`students.dat`) with auto-save on exit |
| **Dynamic Array** | Starts at capacity 10, doubles automatically via `realloc` |
| **Auto Ranking** | Rank recalculated after every add, update, or delete |

---

## Recursive Functions Used

1. `recursiveTotalMarks` — sums marks array recursively
2. `recursiveDisplay` — displays all students recursively
3. `recursiveBinarySearch` — binary search by roll number
4. `recursiveNameSearch` — substring name search (case-insensitive)
5. `recursiveFindMax` — finds highest scorer recursively
6. `recursiveFindMin` — finds lowest scorer recursively
7. `recursiveClassSum` — sums all student totals recursively
8. `recursivePassFail` — counts pass/fail recursively
9. `recursiveSubjectSum` — sums one subject across all students
10. `recursiveQuickSortByMarks` — QuickSort descending by marks
11. `recursiveQuickSortByRoll` — QuickSort ascending by roll number
12. `recursiveGradeDist` — grade bucket distribution counter

---

## Subjects Tracked

- Mathematics
- Physics
- Chemistry
- English
- Computer Science

---

## Grading Scale

| Grade | Percentage |
|---|---|
| A+ | >= 90% |
| A  | >= 80% |
| B  | >= 70% |
| C  | >= 60% |
| D  | >= 50% |
| F  | < 50%  |

---

## Build & Run

### Requirements
- GCC compiler

### Compile
```bash
gcc grade_management_v2.c -o grade_management -Wall -std=c11
```

### Run
```bash
./grade_management        # Linux / macOS
grade_management.exe      # Windows
```

---

## File Structure

```
student-grade-system/
├── grade_management_v2.c   # Full source code (v2 — dynamic + recursive)
├── grade_management.c      # Original cleaned-up version (v1)
├── README.md
└── .gitignore
```

---

## Concepts Demonstrated

- `struct` and arrays of structs
- Pointers and pass-by-reference
- Dynamic memory (`malloc`, `realloc`, `free`)
- Recursive algorithms (search, sort, statistics)
- File I/O (binary read/write with `fread`/`fwrite`)
- Input validation and buffer management
- Modular function design

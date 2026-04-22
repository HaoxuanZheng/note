Here it is — **Packet 9** in clean, printable **Markdown**, matching the structure of Packets 1–8.

---

# 📘 **PACKET 9 — UNIT 8: 2D ARRAYS**  
**Checklist + MCQ Set + FRQ Set + Coding Drills**  
**Print‑Ready Markdown**

---

# 🟦 **UNIT 8 CHECKLIST — 2D ARRAYS**

## ✅ **1. Concepts**
- [ ] 2D array declaration and initialization  
- [ ] Row‑major order  
- [ ] Accessing elements with `grid[r][c]`  
- [ ] Dimensions:  
  - `grid.length` → number of rows  
  - `grid[0].length` → number of columns  
- [ ] Nested loops for traversal  
- [ ] Counting, searching, transforming values  
- [ ] Summing rows/columns  
- [ ] Bounds checking  
- [ ] Common FRQ patterns (Q4 style)  

---

## ✅ **2. Must‑Know Syntax**

### **Declaration**
```java
int[][] grid = new int[3][4];
```

### **Initialization**
```java
int[][] mat = {
    {1, 2, 3},
    {4, 5, 6}
};
```

### **Traversal**
```java
for (int r = 0; r < grid.length; r++) {
    for (int c = 0; c < grid[0].length; c++) {
        System.out.println(grid[r][c]);
    }
}
```

### **Row sum**
```java
int sum = 0;
for (int c = 0; c < grid[r].length; c++) {
    sum += grid[r][c];
}
```

---

## ✅ **3. Common Mistakes**
- [ ] Using `grid.length` for both rows and columns  
- [ ] Swapping row and column indices  
- [ ] Forgetting that rows may have different lengths (jagged arrays)  
- [ ] Off‑by‑one errors in nested loops  
- [ ] Incorrectly summing rows vs. columns  
- [ ] Using enhanced for‑loop incorrectly when indices are needed  

---

## ✅ **4. Mini‑Patterns**

### **Count matches**
```java
int count = 0;
for (int r = 0; r < grid.length; r++) {
    for (int c = 0; c < grid[0].length; c++) {
        if (grid[r][c] == target) count++;
    }
}
```

### **Find max**
```java
int max = grid[0][0];
for (int r = 0; r < grid.length; r++) {
    for (int c = 0; c < grid[0].length; c++) {
        if (grid[r][c] > max) max = grid[r][c];
    }
}
```

### **Row sum**
```java
int sum = 0;
for (int c = 0; c < grid[r].length; c++) sum += grid[r][c];
```

---

# 🟩 **UNIT 8 PRACTICE SET A — MCQ (15 QUESTIONS)**  
*(Answer key at bottom)*

### **1.** What is printed?
```java
int[][] a = {{1, 2}, {3, 4}};
System.out.println(a[0][1]);
```
A. 1  
B. 2  
C. 3  
D. 4  

---

### **2.** What is printed?
```java
int[][] a = new int[2][3];
System.out.println(a.length);
```
A. 2  
B. 3  
C. 5  
D. Error  

---

### **3.** What is printed?
```java
int[][] a = new int[2][3];
System.out.println(a[0].length);
```
A. 2  
B. 3  
C. 5  
D. Error  

---

### **4.** What is printed?
```java
int[][] a = {{1, 2, 3}, {4, 5, 6}};
System.out.println(a[1][0]);
```
A. 1  
B. 2  
C. 4  
D. 5  

---

### **5.** What is printed?
```java
int[][] a = {{1, 2}, {3, 4}};
int sum = 0;
for (int r = 0; r < a.length; r++) {
    for (int c = 0; c < a[0].length; c++) {
        sum += a[r][c];
    }
}
System.out.println(sum);
```
A. 4  
B. 6  
C. 8  
D. 10  

---

### **6.** What is printed?
```java
int[][] a = {{2, 4}, {6, 8}};
System.out.println(a[1][1]);
```
A. 2  
B. 4  
C. 6  
D. 8  

---

### **7.** What is printed?
```java
int[][] a = {{1, 2, 3}, {4, 5, 6}};
System.out.println(a[0].length);
```
A. 2  
B. 3  
C. 6  
D. Error  

---

### **8.** What is printed?
```java
int[][] a = {{1}, {2}, {3}};
System.out.println(a.length);
```
A. 1  
B. 2  
C. 3  
D. Error  

---

### **9.** What is printed?
```java
int[][] a = {{1, 2}, {3, 4}};
System.out.println(a[1][2]);
```
A. 2  
B. 3  
C. 4  
D. Error  

---

### **10.** What is printed?
```java
int[][] a = {{1, 2}, {3, 4}};
for (int r = 0; r < a.length; r++) {
    System.out.print(a[r][0]);
}
```
A. 13  
B. 24  
C. 12  
D. 34  

---

### **11.** What is printed?
```java
int[][] a = {{1, 2}, {3, 4}};
for (int r = 0; r < a.length; r++) {
    for (int c = 0; c < a[0].length; c++) {
        System.out.print(a[r][c]);
    }
}
```
A. 1234  
B. 1324  
C. 2143  
D. 4321  

---

### **12.** What is printed?
```java
int[][] a = {{5, 1}, {2, 9}};
int max = a[0][0];
for (int r = 0; r < a.length; r++) {
    for (int c = 0; c < a[0].length; c++) {
        if (a[r][c] > max) max = a[r][c];
    }
}
System.out.println(max);
```
A. 1  
B. 2  
C. 5  
D. 9  

---

### **13.** What is printed?
```java
int[][] a = {{1, 2}, {3, 4}};
System.out.println(a[0].length + a.length);
```
A. 2  
B. 3  
C. 4  
D. 5  

---

### **14.** What is printed?
```java
int[][] a = {{1, 2, 3}};
System.out.println(a[0][2]);
```
A. 1  
B. 2  
C. 3  
D. Error  

---

### **15.** What is printed?
```java
int[][] a = {{1, 2}, {3, 4}};
int count = 0;
for (int r = 0; r < a.length; r++) {
    for (int c = 0; c < a[0].length; c++) {
        if (a[r][c] % 2 == 0) count++;
    }
}
System.out.println(count);
```
A. 1  
B. 2  
C. 3  
D. 4  

---

# 🟧 **UNIT 8 PRACTICE SET B — FRQ‑STYLE TASKS**

### **FRQ 1 — Count Greater Than**
Write a method that returns how many values in a 2D array are **greater than** a given limit.

```java
public static int countGreater(int[][] grid, int limit)
```

---

### **FRQ 2 — Row Sum**
Return the **sum** of all values in a given row.  
If the row index is invalid, return `-1`.

```java
public static int rowSum(int[][] grid, int row)
```

---

### **FRQ 3 — Column Max**
Return the **maximum value** in a given column.

```java
public static int columnMax(int[][] grid, int col)
```

---

# 🟪 **UNIT 8 PRACTICE SET C — CODING DRILLS**

### **Drill 1 — Fill in the blank**
```java
int rows = grid.________;
int cols = grid[0].________;
```

---

### **Drill 2 — Predict the output**
```java
int[][] a = {{1, 2}, {3, 4}};
System.out.println(a[1][0]);
```

---

### **Drill 3 — Fix the bug**
```java
for (int r = 0; r <= grid.length; r++) {   // fix this
    for (int c = 0; c < grid[0].length; c++) {
        System.out.println(grid[r][c]);
    }
}
```

---

### **Drill 4 — Write a loop**
Print all elements in **row 2** of `grid`.

---

### **Drill 5 — Diagonal sum**
Write code to compute the sum of the **main diagonal** of a square matrix.

---

# 🟫 **ANSWER KEY (MCQ)**  
1. B  
2. A  
3. B  
4. C  
5. C  
6. D  
7. B  
8. C  
9. D  
10. A  
11. A  
12. D  
13. D  
14. C  
15. B  

---

# ✅ **PACKET 9 COMPLETE**

If you'd like, I can now generate:

### **Packet 10 — Unit 9: Inheritance (Checklist + MCQ + FRQ + Drills)**  
*(Note: Inheritance is enrichment in the new CED but still useful.)*

Just say: **Generate Packet 10.**
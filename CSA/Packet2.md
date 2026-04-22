Got it — here is **Packet 2** in clean, printable **Markdown**, matching the structure of Packet 1.

---

# 📘 **PACKET 2 — UNIT 1: PRIMITIVE TYPES**  
**Checklist + MCQ Set + FRQ Set + Coding Drills**  
**Print‑Ready Markdown**

---

# 🟦 **UNIT 1 CHECKLIST — PRIMITIVE TYPES**

## ✅ **1. Concepts**
- [ ] Primitive types: `int`, `double`, `boolean`, `char`  
- [ ] Variable declaration & initialization  
- [ ] Assignment & reassignment  
- [ ] Arithmetic operators: `+`, `-`, `*`, `/`, `%`  
- [ ] Integer vs. double division  
- [ ] Casting (widening vs. narrowing)  
- [ ] Operator precedence  
- [ ] Overflow behavior  
- [ ] `final` constants  

---

## ✅ **2. Must‑Know Syntax**
```java
int x = 5;
double y = 3.14;
boolean flag = true;
char letter = 'A';

int a = 5 / 2;      // 2
double b = 5 / 2.0; // 2.5

int n = (int) 7.9;  // 7
final double PI = 3.14159;
```

---

## ✅ **3. Common Mistakes**
- [ ] Expecting `5 / 2` to be `2.5`  
- [ ] Forgetting to initialize variables  
- [ ] Using `'A'` vs `"A"` incorrectly (`char` vs `String`)  
- [ ] Misusing `%` (modulo)  
- [ ] Overflow not throwing an error (`int` wraps around)  

---

## ✅ **4. Mini‑Patterns**
### **Modulo patterns**
- `n % 2 == 0` → even  
- `n % 10` → last digit  
- `(n / 10) % 10` → second‑to‑last digit  

### **Casting patterns**
```java
(double) a / b
(int) (x * 100)
```

---

# 🟩 **UNIT 1 PRACTICE SET A — MCQ (15 QUESTIONS)**  
*(Answer key at bottom)*

### **1.** What is the value of `7 / 2`?  
A. 3  
B. 3.0  
C. 3.5  
D. 4  

### **2.** What is the value of `7 / 2.0`?  
A. 3  
B. 3.0  
C. 3.5  
D. 4  

### **3.** What is the value of `7 % 3`?  
A. 0  
B. 1  
C. 2  
D. 3  

### **4.** What is printed?
```java
int x = 3;
x = x + 2 * 4;
System.out.println(x);
```
A. 11  
B. 20  
C. 14  
D. 8  

### **5.** What is printed?
```java
double d = (int)(7.8 + 0.2);
System.out.println(d);
```
A. 7  
B. 8  
C. 7.8  
D. 8.0  

### **6.** Which is a valid `char` literal?  
A. `"A"`  
B. `'AB'`  
C. `'A'`  
D. `"@"`  

### **7.** What is the value of:
```java
int x = 10;
x = x % 4;
```
A. 0  
B. 1  
C. 2  
D. 3  

### **8.** What is printed?
```java
System.out.println(3 + 4 * 2);
```
A. 14  
B. 11  
C. 16  
D. 8  

### **9.** What is printed?
```java
System.out.println((int)(3.9) + 1);
```
A. 3  
B. 4  
C. 5  
D. 3.9  

### **10.** What is printed?
```java
int a = 2;
int b = 3;
double c = a / b;
System.out.println(c);
```
A. 0  
B. 0.0  
C. 0.666…  
D. 1.5  

### **11.** Which expression evaluates to a `double`?  
A. `5 / 2`  
B. `5 / 2.0`  
C. `(int)(5 / 2)`  
D. `5 % 2`  

### **12.** What is printed?
```java
int x = 1;
x += 3 * 2;
System.out.println(x);
```
A. 7  
B. 8  
C. 5  
D. 6  

### **13.** What is printed?
```java
System.out.println(10 % 4 * 2);
```
A. 0  
B. 2  
C. 4  
D. 12  

### **14.** What is printed?
```java
System.out.println((int)(2.5) + (int)(2.5));
```
A. 4  
B. 5  
C. 6  
D. 2  

### **15.** What is printed?
```java
int x = 1000000;
x = x * x;
System.out.println(x);
```
A. 1,000,000,000,000  
B. Overflow  
C. A negative number  
D. Compile error  

---

# 🟧 **UNIT 1 PRACTICE SET B — FRQ‑STYLE TASKS**

### **FRQ 1 — Digit Sum**
Write a method that returns the **sum of the digits** of a positive integer.

```java
public static int digitSum(int n)
```

**Example:**  
`digitSum(472)` → `13`

---

### **FRQ 2 — Count Even**
Write a method that counts how many numbers in an `int[]` are even.

```java
public static int countEven(int[] arr)
```

---

### **FRQ 3 — Normalize Score**
Given a score out of 50, return the percentage as a `double`.

```java
public static double normalize(int score)
```

Example:  
`normalize(25)` → `50.0`

---

# 🟪 **UNIT 1 PRACTICE SET C — CODING DRILLS**

### **Drill 1 — Fill in the blank**
```java
int x = 17;
int lastDigit = x % __;
```

### **Drill 2 — Predict the output**
```java
System.out.println((int)(6.9) - 2);
```

### **Drill 3 — Fix the bug**
```java
char letter = "A";   // fix this
```

### **Drill 4 — Rewrite using casting**
Rewrite so the result is `2.5`:
```java
System.out.println(5 / 2);
```

### **Drill 5 — Overflow check**
Explain why this prints a negative number:
```java
int x = 50000 * 50000;
System.out.println(x);
```

---

# 🟫 **ANSWER KEY (MCQ)**  
1. A  
2. C  
3. B  
4. A  
5. B  
6. C  
7. C  
8. B  
9. C  
10. B  
11. B  
12. A  
13. C  
14. A  
15. C  

---

# ✅ **PACKET 2 COMPLETE**

If you want, I can now generate:

### **Packet 3 — Unit 2: Using Objects (Checklist + MCQ + FRQ + Drills)**

Just say: **Generate Packet 3.**
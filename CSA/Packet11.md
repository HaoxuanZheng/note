Here it is — **Packet 11**, the final packet in the AP CSA Unit Series, in clean, printable **Markdown**, matching the structure of Packets 1–10.

> **Note:** Recursion is *enrichment* in the new AP CSA CED (2025–26), but it remains extremely valuable for algorithmic thinking and appears in many AP‑style practice resources. This packet keeps recursion AP‑aligned and beginner‑friendly.

---

# 📘 **PACKET 11 — UNIT 10: RECURSION (ENRICHMENT)**  
**Checklist + MCQ Set + FRQ Set + Coding Drills**  
**Print‑Ready Markdown**

---

# 🟦 **UNIT 10 CHECKLIST — RECURSION**

## ✅ **1. Concepts**
- [ ] Definition of recursion  
- [ ] Base case vs. recursive case  
- [ ] How recursive calls build a call stack  
- [ ] How to trace recursive calls  
- [ ] When recursion stops  
- [ ] Common recursive patterns:  
  - Sum of digits  
  - Factorial  
  - Fibonacci  
  - Reverse string  
  - Count occurrences  
- [ ] Avoiding infinite recursion  
- [ ] Understanding stack overflow  

---

## ✅ **2. Must‑Know Syntax**

### **Basic recursive structure**
```java
public static int f(int n) {
    if (n == 0) {        // base case
        return 1;
    } else {             // recursive case
        return n * f(n - 1);
    }
}
```

### **String recursion**
```java
public static String reverse(String s) {
    if (s.length() <= 1) return s;
    return reverse(s.substring(1)) + s.charAt(0);
}
```

### **Counting recursion**
```java
public static int countX(String s) {
    if (s.length() == 0) return 0;
    if (s.charAt(0) == 'x') return 1 + countX(s.substring(1));
    return countX(s.substring(1));
}
```

---

## ✅ **3. Common Mistakes**
- [ ] Missing or incorrect base case  
- [ ] Base case that never triggers  
- [ ] Forgetting to return the recursive call  
- [ ] Changing the string incorrectly (substring errors)  
- [ ] Infinite recursion due to wrong parameter update  
- [ ] Confusing recursion with iteration  

---

## ✅ **4. Mini‑Patterns**

### **Decreasing integer recursion**
```java
f(n) → f(n - 1)
```

### **Shrinking string recursion**
```java
f(s) → f(s.substring(1))
```

### **Divide‑and‑conquer**
```java
f(n) → f(n/2)
```

---

# 🟩 **UNIT 10 PRACTICE SET A — MCQ (15 QUESTIONS)**  
*(Answer key at bottom)*

### **1.** What is printed?
```java
public static int f(int n) {
    if (n == 0) return 1;
    return 2 * f(n - 1);
}
System.out.println(f(3));
```
A. 2  
B. 4  
C. 6  
D. 8  

---

### **2.** What is printed?
```java
public static int f(int n) {
    if (n == 1) return 1;
    return n + f(n - 1);
}
System.out.println(f(3));
```
A. 3  
B. 4  
C. 5  
D. 6  

---

### **3.** What is printed?
```java
public static void f(int n) {
    if (n == 0) return;
    System.out.print(n);
    f(n - 1);
}
f(3);
```
A. 321  
B. 123  
C. 3  
D. 0  

---

### **4.** What is printed?
```java
public static int f(int n) {
    if (n <= 1) return n;
    return f(n - 1) + f(n - 2);
}
System.out.println(f(4));
```
A. 2  
B. 3  
C. 5  
D. 8  

---

### **5.** What is printed?
```java
public static int f(int n) {
    if (n == 0) return 0;
    return 1 + f(n - 1);
}
System.out.println(f(4));
```
A. 1  
B. 2  
C. 3  
D. 4  

---

### **6.** What is printed?
```java
public static String f(String s) {
    if (s.length() == 0) return "";
    return f(s.substring(1)) + s.charAt(0);
}
System.out.println(f("ab"));
```
A. "ab"  
B. "ba"  
C. "a"  
D. ""  

---

### **7.** What is printed?
```java
public static int f(int n) {
    if (n == 1) return 1;
    return f(n - 1) * 2;
}
System.out.println(f(4));
```
A. 2  
B. 4  
C. 6  
D. 8  

---

### **8.** What is printed?
```java
public static int f(int n) {
    if (n == 0) return 10;
    return f(n - 1) + 1;
}
System.out.println(f(3));
```
A. 10  
B. 11  
C. 12  
D. 13  

---

### **9.** What is printed?
```java
public static int f(int n) {
    if (n == 0) return 1;
    return n * f(n - 1);
}
System.out.println(f(3));
```
A. 3  
B. 6  
C. 9  
D. 12  

---

### **10.** What is printed?
```java
public static void f(int n) {
    if (n == 0) return;
    f(n - 1);
    System.out.print(n);
}
f(3);
```
A. 321  
B. 123  
C. 3  
D. 12  

---

### **11.** What is printed?
```java
public static int f(int n) {
    if (n <= 1) return 1;
    return f(n - 1) + f(n - 1);
}
System.out.println(f(3));
```
A. 2  
B. 4  
C. 6  
D. 8  

---

### **12.** What is printed?
```java
public static int f(int n) {
    if (n == 0) return 5;
    return f(n - 1);
}
System.out.println(f(4));
```
A. 0  
B. 1  
C. 4  
D. 5  

---

### **13.** What is printed?
```java
public static int f(int n) {
    if (n == 0) return 0;
    if (n % 2 == 0) return 1 + f(n - 1);
    return f(n - 1);
}
System.out.println(f(5));
```
A. 1  
B. 2  
C. 3  
D. 4  

---

### **14.** What is printed?
```java
public static int f(int n) {
    if (n == 0) return 1;
    return f(n - 1) * 3;
}
System.out.println(f(2));
```
A. 3  
B. 6  
C. 9  
D. 27  

---

### **15.** What is printed?
```java
public static int f(int n) {
    if (n == 0) return 0;
    return f(n - 1) + n;
}
System.out.println(f(3));
```
A. 3  
B. 4  
C. 5  
D. 6  

---

# 🟧 **UNIT 10 PRACTICE SET B — FRQ‑STYLE TASKS**

### **FRQ 1 — Sum of Digits (Recursive)**
Write a recursive method that returns the sum of the digits of `n`.

```java
public static int digitSum(int n)
```

Example:  
`digitSum(472)` → `13`

---

### **FRQ 2 — Count Character**
Write a recursive method that counts how many times a character appears in a string.

```java
public static int countChar(String s, char ch)
```

---

### **FRQ 3 — Remove Character**
Write a recursive method that returns a new string with all occurrences of `ch` removed.

```java
public static String removeChar(String s, char ch)
```

Example:  
`removeChar("banana", 'a')` → `"bnn"`

---

# 🟪 **UNIT 10 PRACTICE SET C — CODING DRILLS**

### **Drill 1 — Fill in the blank**
```java
if (n == 0) return ______;
```

---

### **Drill 2 — Predict the output**
```java
System.out.println(f("cat"));
```
Where:
```java
public static String f(String s) {
    if (s.length() <= 1) return s;
    return f(s.substring(1)) + s.charAt(0);
}
```

---

### **Drill 3 — Fix the bug**
```java
public static int f(int n) {
    return f(n - 1);   // missing base case
}
```

---

### **Drill 4 — Write a recursive method**
Write a recursive method that returns the number of uppercase letters in a string.

---

### **Drill 5 — Trace the recursion**
Trace:
```java
f(3)
```
Where:
```java
public static void f(int n) {
    if (n == 0) return;
    System.out.print(n);
    f(n - 1);
}
```

---

# 🟫 **ANSWER KEY (MCQ)**  
1. D  
2. D  
3. A  
4. C  
5. D  
6. B  
7. D  
8. D  
9. B  
10. B  
11. B  
12. D  
13. B  
14. C  
15. D  

---

# ✅ **PACKET 11 COMPLETE**

If you want, I can now generate:

### ⭐ **The Final Combined Review Packet**  
(“AP CSA Final Review: 100 MCQs + 12 FRQs + Algorithms + Cheat Sheets”)

Just say: **Generate Final Review Packet.**
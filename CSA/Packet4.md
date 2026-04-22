Here it is — **Packet 4** in clean, printable **Markdown**, matching the structure of Packets 1–3.

---

# 📘 **PACKET 4 — UNIT 3: BOOLEAN EXPRESSIONS & IF STATEMENTS**  
**Checklist + MCQ Set + FRQ Set + Coding Drills**  
**Print‑Ready Markdown**

---

# 🟦 **UNIT 3 CHECKLIST — BOOLEAN EXPRESSIONS & IF STATEMENTS**

## ✅ **1. Concepts**
- [ ] Relational operators: `==`, `!=`, `<`, `>`, `<=`, `>=`  
- [ ] Logical operators: `&&`, `||`, `!`  
- [ ] Short‑circuit evaluation  
- [ ] Boolean expressions with variables and method calls  
- [ ] `if`, `if‑else`, `if‑else‑if` chains  
- [ ] Nested conditionals  
- [ ] Truth tables  
- [ ] De Morgan’s Laws  
- [ ] Order of evaluation  

---

## ✅ **2. Must‑Know Syntax**
### **Basic conditional**
```java
if (condition) {
    // code
}
```

### **If‑else**
```java
if (condition) {
} else {
}
```

### **If‑else‑if chain**
```java
if (a > 10) {
} else if (a > 5) {
} else {
}
```

### **Boolean logic**
```java
if (x > 0 && y < 10)
if (a == b || c != d)
if (!(x > 0))
```

### **De Morgan’s Laws**
```java
!(A && B)  ==  !A || !B
!(A || B)  ==  !A && !B
```

---

## ✅ **3. Common Mistakes**
- [ ] Using `=` instead of `==`  
- [ ] Using `==` to compare Strings (should use `.equals`)  
- [ ] Misunderstanding short‑circuiting  
- [ ] Incorrect ordering in `if‑else‑if` chains  
- [ ] Forgetting that only the **nearest** `if` pairs with an `else`  
- [ ] Over‑parenthesizing or under‑parenthesizing expressions  

---

## ✅ **4. Mini‑Patterns**
### **Range check**
```java
if (x >= 1 && x <= 10)
```

### **Exclusive OR (XOR) pattern**
```java
if ((a && !b) || (!a && b))
```

### **Check if a character is a vowel**
```java
if ("aeiouAEIOU".indexOf(ch) != -1)
```

---

# 🟩 **UNIT 3 PRACTICE SET A — MCQ (15 QUESTIONS)**  
*(Answer key at bottom)*

### **1.** What is printed?
```java
System.out.println(5 > 3 && 2 < 1);
```
A. true  
B. false  
C. 1  
D. 0  

---

### **2.** What is printed?
```java
System.out.println(!(4 == 4));
```
A. true  
B. false  
C. 4  
D. Error  

---

### **3.** What is printed?
```java
int x = 7;
System.out.println(x > 5 || x < 0);
```
A. true  
B. false  
C. Depends  
D. Error  

---

### **4.** What is printed?
```java
int a = 3, b = 4;
System.out.println(a == 3 && b == 5);
```
A. true  
B. false  
C. 3  
D. 5  

---

### **5.** What is printed?
```java
System.out.println(true || false && false);
```
A. true  
B. false  
C. Error  
D. Depends  

---

### **6.** What is printed?
```java
int x = 10;
if (x > 5)
    if (x < 20)
        System.out.println("A");
    else
        System.out.println("B");
```
A. A  
B. B  
C. Nothing  
D. Error  

---

### **7.** What is printed?
```java
int x = 5;
if (x > 10)
    System.out.println("big");
else if (x > 3)
    System.out.println("medium");
else
    System.out.println("small");
```
A. big  
B. medium  
C. small  
D. Error  

---

### **8.** What is printed?
```java
System.out.println(!(false || true));
```
A. true  
B. false  
C. Error  
D. 0  

---

### **9.** What is printed?
```java
int x = 3;
System.out.println(x == 3 || x / 0 == 1);
```
A. true  
B. false  
C. Error  
D. Depends  

---

### **10.** What is printed?
```java
int x = 8;
System.out.println(x % 2 == 0 && x % 4 == 0);
```
A. true  
B. false  
C. 8  
D. Error  

---

### **11.** What is printed?
```java
boolean a = true, b = false;
System.out.println(a && !b);
```
A. true  
B. false  
C. Error  
D. 0  

---

### **12.** What is printed?
```java
int x = 4;
System.out.println(x > 1 && x < 4);
```
A. true  
B. false  
C. Error  
D. Depends  

---

### **13.** What is printed?
```java
System.out.println(!true || false);
```
A. true  
B. false  
C. Error  
D. 1  

---

### **14.** What is printed?
```java
int x = 5;
if (x > 10)
    System.out.println("A");
System.out.println("B");
```
A. A  
B. B  
C. A B  
D. Nothing  

---

### **15.** What is printed?
```java
int x = 7;
if (x > 0)
    if (x > 10)
        System.out.println("big");
    else
        System.out.println("medium");
else
    System.out.println("small");
```
A. big  
B. medium  
C. small  
D. Error  

---

# 🟧 **UNIT 3 PRACTICE SET B — FRQ‑STYLE TASKS**

### **FRQ 1 — Count Matches**
Write a method that counts how many elements in an `int[]` are **between** `low` and `high` inclusive.

```java
public static int countInRange(int[] arr, int low, int high)
```

---

### **FRQ 2 — Password Strength**
A password is considered strong if:
- It has at least 8 characters  
- It contains `'@'` or `'#'`  
- It does **not** contain spaces  

Write:
```java
public static boolean isStrong(String pwd)
```

---

### **FRQ 3 — Closest to Zero**
Given two integers, return the one **closest to zero**.  
If tied, return the **positive** one.

```java
public static int closestToZero(int a, int b)
```

Examples:  
`closestToZero(3, -2)` → `-2`  
`closestToZero(-5, 5)` → `5`

---

# 🟪 **UNIT 3 PRACTICE SET C — CODING DRILLS**

### **Drill 1 — Fill in the blank**
```java
if (x >= 1 && x <= 10) {
    System.out.println("in range");
}
```
Fill in: `x >= __ && x <= __`

---

### **Drill 2 — Predict the output**
```java
System.out.println(!(true && false));
```

---

### **Drill 3 — Fix the bug**
```java
String s = "hello";
if (s == "hello") {   // fix this
    System.out.println("match");
}
```

---

### **Drill 4 — Rewrite using De Morgan**
Rewrite:
```java
!(x > 0 && y > 0)
```

---

### **Drill 5 — Nested if rewrite**
Rewrite this as a single Boolean expression:
```java
if (x > 0) {
    if (x < 100) {
        return true;
    }
}
return false;
```

---

# 🟫 **ANSWER KEY (MCQ)**  
1. B  
2. B  
3. A  
4. B  
5. A  
6. A  
7. B  
8. B  
9. A  
10. A  
11. A  
12. B  
13. A  
14. B  
15. B  

---

# ✅ **PACKET 4 COMPLETE**

If you'd like, I can now generate:

### **Packet 5 — Unit 4: Iteration (Checklist + MCQ + FRQ + Drills)**

Just say: **Generate Packet 5.**
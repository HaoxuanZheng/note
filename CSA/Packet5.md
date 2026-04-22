Here it is — **Packet 5** in clean, printable **Markdown**, matching the structure of Packets 1–4.

---

# 📘 **PACKET 5 — UNIT 4: ITERATION**  
**Checklist + MCQ Set + FRQ Set + Coding Drills**  
**Print‑Ready Markdown**

---

# 🟦 **UNIT 4 CHECKLIST — ITERATION**

## ✅ **1. Concepts**
- [ ] `while` loops  
- [ ] `for` loops  
- [ ] Loop control variables (init → condition → update)  
- [ ] Off‑by‑one errors  
- [ ] Infinite loops  
- [ ] Nested loops  
- [ ] Loop invariants (what changes vs. what stays constant)  
- [ ] String traversal with loops  
- [ ] Accumulator patterns (sum, count, max/min)  
- [ ] Early return inside loops  

---

## ✅ **2. Must‑Know Syntax**

### **For loop**
```java
for (int i = 0; i < n; i++) {
    // body
}
```

### **While loop**
```java
int i = 0;
while (i < n) {
    // body
    i++;
}
```

### **String traversal**
```java
for (int i = 0; i < s.length(); i++) {
    char c = s.charAt(i);
}
```

### **Nested loops**
```java
for (int r = 0; r < rows; r++) {
    for (int c = 0; c < cols; c++) {
        // body
    }
}
```

---

## ✅ **3. Common Mistakes**
- [ ] Forgetting to update loop variable → infinite loop  
- [ ] Using `<= s.length()` instead of `< s.length()`  
- [ ] Updating the wrong variable in nested loops  
- [ ] Using `i++` inside an `if` accidentally  
- [ ] Incorrectly mixing `while` and `for` logic  
- [ ] Off‑by‑one errors in ranges  

---

## ✅ **4. Mini‑Patterns**

### **Count pattern**
```java
int count = 0;
for (int i = 0; i < arr.length; i++) {
    if (condition) count++;
}
```

### **Sum pattern**
```java
int sum = 0;
for (int i = 0; i < arr.length; i++) {
    sum += arr[i];
}
```

### **Max pattern**
```java
int max = arr[0];
for (int i = 1; i < arr.length; i++) {
    if (arr[i] > max) max = arr[i];
}
```

### **Reverse traversal**
```java
for (int i = s.length() - 1; i >= 0; i--) {
}
```

---

# 🟩 **UNIT 4 PRACTICE SET A — MCQ (15 QUESTIONS)**  
*(Answer key at bottom)*

### **1.** What is printed?
```java
for (int i = 0; i < 5; i++) {
    System.out.print(i + " ");
}
```
A. `0 1 2 3 4`  
B. `1 2 3 4 5`  
C. `0 1 2 3 4 5`  
D. Infinite loop  

---

### **2.** What is printed?
```java
int i = 3;
while (i > 0) {
    System.out.print(i);
    i--;
}
```
A. `321`  
B. `012`  
C. `210`  
D. `123`  

---

### **3.** How many times does the loop run?
```java
for (int i = 2; i <= 10; i += 2) { }
```
A. 4  
B. 5  
C. 6  
D. 8  

---

### **4.** What is printed?
```java
String s = "abcd";
for (int i = 1; i < s.length(); i++) {
    System.out.print(s.charAt(i));
}
```
A. `abcd`  
B. `bcd`  
C. `abc`  
D. `cd`  

---

### **5.** What is printed?
```java
int x = 0;
while (x < 3) {
    x++;
}
System.out.println(x);
```
A. 0  
B. 1  
C. 2  
D. 3  

---

### **6.** What is printed?
```java
for (int i = 5; i > 0; i -= 2) {
    System.out.print(i + " ");
}
```
A. `5 3 1`  
B. `5 4 3 2 1`  
C. `5 3`  
D. `3 1`  

---

### **7.** What is printed?
```java
int count = 0;
for (int i = 0; i < 4; i++) {
    for (int j = 0; j < 2; j++) {
        count++;
    }
}
System.out.println(count);
```
A. 4  
B. 6  
C. 8  
D. 10  

---

### **8.** What is printed?
```java
String s = "hello";
int count = 0;
for (int i = 0; i < s.length(); i++) {
    if (s.charAt(i) == 'l') count++;
}
System.out.println(count);
```
A. 0  
B. 1  
C. 2  
D. 3  

---

### **9.** What is printed?
```java
int i = 0;
while (i < 3) {
    System.out.print(i);
    i += 2;
}
```
A. `0 2`  
B. `0 1 2`  
C. `0 2 4`  
D. `0 2` (no space)  

---

### **10.** What is printed?
```java
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < i; j++) {
        System.out.print("*");
    }
}
```
A. `***`  
B. `* **`  
C. `**`  
D. `* **` (no spaces)  

---

### **11.** What is printed?
```java
int x = 10;
while (x < 10) {
    x++;
}
System.out.println(x);
```
A. 10  
B. 11  
C. Infinite loop  
D. Nothing  

---

### **12.** What is printed?
```java
for (int i = 3; i >= 0; i--) {
    System.out.print(i);
}
```
A. `0123`  
B. `3210`  
C. `4321`  
D. `1234`  

---

### **13.** What is printed?
```java
String s = "java";
for (int i = 0; i < s.length() - 1; i++) {
    System.out.print(s.charAt(i));
}
```
A. `java`  
B. `jav`  
C. `ava`  
D. `ja`  

---

### **14.** What is printed?
```java
int sum = 0;
for (int i = 1; i <= 3; i++) {
    sum += i;
}
System.out.println(sum);
```
A. 3  
B. 4  
C. 5  
D. 6  

---

### **15.** What is printed?
```java
int x = 1;
while (x < 20) {
    x *= 2;
}
System.out.println(x);
```
A. 8  
B. 16  
C. 32  
D. Infinite loop  

---

# 🟧 **UNIT 4 PRACTICE SET B — FRQ‑STYLE TASKS**

### **FRQ 1 — Count Digits**
Write a method that counts how many characters in a string are digits (`'0'`–`'9'`).

```java
public static int countDigits(String s)
```

---

### **FRQ 2 — First Even**
Return the **first even number** in an array.  
If none exist, return `-1`.

```java
public static int firstEven(int[] arr)
```

---

### **FRQ 3 — Reverse String**
Return a **new string** that is the reverse of the input.

```java
public static String reverse(String s)
```

Example:  
`reverse("cat")` → `"tac"`

---

# 🟪 **UNIT 4 PRACTICE SET C — CODING DRILLS**

### **Drill 1 — Fill in the blank**
```java
for (int i = 0; i < s.______; i++) {
    char c = s.charAt(i);
}
```

---

### **Drill 2 — Predict the output**
```java
int x = 0;
while (x < 3) {
    System.out.print(x);
    x++;
}
```

---

### **Drill 3 — Fix the bug**
```java
int i = 0;
while (i < 5) {
    System.out.println(i);
    // missing update
}
```

---

### **Drill 4 — Rewrite using a for loop**
Rewrite:
```java
int i = 10;
while (i >= 0) {
    System.out.println(i);
    i--;
}
```

---

### **Drill 5 — Nested loop trace**
Predict the output:
```java
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 2; j++) {
        System.out.print(i + "" + j + " ");
    }
}
```

---

# 🟫 **ANSWER KEY (MCQ)**  
1. A  
2. A  
3. B  
4. B  
5. D  
6. A  
7. C  
8. C  
9. D  
10. D  
11. A  
12. B  
13. B  
14. D  
15. C  

---

# ✅ **PACKET 5 COMPLETE**

If you'd like, I can now generate:

### **Packet 6 — Unit 5: Writing Classes (Checklist + MCQ + FRQ + Drills)**

Just say: **Generate Packet 6.**
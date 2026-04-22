Here it is — **Packet 3** in clean, printable **Markdown**, matching the structure of Packets 1 and 2.

---

# 📘 **PACKET 3 — UNIT 2: USING OBJECTS**  
**Checklist + MCQ Set + FRQ Set + Coding Drills**  
**Print‑Ready Markdown**

---

# 🟦 **UNIT 2 CHECKLIST — USING OBJECTS**

## ✅ **1. Concepts**
- [ ] Difference between **class** and **object**  
- [ ] Creating objects with `new`  
- [ ] Calling methods on objects  
- [ ] Return values vs. void methods  
- [ ] Passing parameters to methods  
- [ ] Understanding **reference types**  
- [ ] Using the **Java Quick Reference** (`String`, `Math`)  
- [ ] String immutability  
- [ ] Autoboxing basics (`Integer`, `Double`)  

---

## ✅ **2. Must‑Know Syntax**
### **Object creation**
```java
String s = new String("hello"); // rarely used
String t = "hello";             // preferred
Random r = new Random();
```

### **Method calls**
```java
int len = t.length();
String sub = t.substring(1, 4);
int idx = t.indexOf("lo");
```

### **Math class**
```java
double x = Math.sqrt(25);
int m = Math.max(3, 7);
double r = Math.random(); // 0.0 <= r < 1.0
```

---

## ✅ **3. Common Mistakes**
- [ ] Using `==` instead of `.equals()` for Strings  
- [ ] Assuming `String` methods modify the original string  
- [ ] Mixing up `substring(begin, end)` (end is **exclusive**)  
- [ ] Forgetting that `Math` methods are **static**  
- [ ] Passing wrong parameter types to methods  

---

## ✅ **4. Mini‑Patterns**
### **String traversal**
```java
for (int i = 0; i < s.length(); i++) {
    char c = s.charAt(i);
}
```

### **Substring extraction**
```java
String first = s.substring(0, 1);
String last3 = s.substring(s.length() - 3);
```

### **Random integer in range**
```java
int roll = (int)(Math.random() * 6) + 1; // 1–6
```

---

# 🟩 **UNIT 2 PRACTICE SET A — MCQ (15 QUESTIONS)**  
*(Answer key at bottom)*

### **1.** What is printed?
```java
String s = "hello";
System.out.println(s.length());
```
A. 4  
B. 5  
C. 6  
D. Error  

---

### **2.** What is printed?
```java
String s = "banana";
System.out.println(s.indexOf("na"));
```
A. 1  
B. 2  
C. 3  
D. -1  

---

### **3.** What is printed?
```java
String s = "computer";
System.out.println(s.substring(3, 6));
```
A. "put"  
B. "put e"  
C. "puter"  
D. "com"  

---

### **4.** What is printed?
```java
String s = "abc";
s.toUpperCase();
System.out.println(s);
```
A. "ABC"  
B. "abc"  
C. "Abc"  
D. Error  

---

### **5.** What is printed?
```java
System.out.println("dog".compareTo("cat"));
```
A. Negative number  
B. Zero  
C. Positive number  
D. Error  

---

### **6.** What is printed?
```java
System.out.println(Math.sqrt(49));
```
A. 7  
B. 7.0  
C. 49  
D. 49.0  

---

### **7.** What is printed?
```java
System.out.println((int)(Math.random() * 3));
```
A. Always 0  
B. 0, 1, or 2  
C. 1, 2, or 3  
D. 0 or 1  

---

### **8.** What is printed?
```java
String s = "hello";
System.out.println(s.substring(1));
```
A. "h"  
B. "ello"  
C. "llo"  
D. "o"  

---

### **9.** What is printed?
```java
String s = "racecar";
System.out.println(s.charAt(3));
```
A. 'c'  
B. 'e'  
C. 'a'  
D. 'r'  

---

### **10.** What is printed?
```java
String a = "hi";
String b = "hi";
System.out.println(a == b);
```
A. true  
B. false  
C. Depends  
D. Error  

---

### **11.** What is printed?
```java
String s = "abcdef";
System.out.println(s.substring(2, 2));
```
A. "c"  
B. ""  
C. "bc"  
D. Error  

---

### **12.** What is printed?
```java
System.out.println("apple".compareTo("banana") < 0);
```
A. true  
B. false  
C. Depends  
D. Error  

---

### **13.** What is printed?
```java
String s = "hello";
System.out.println(s.indexOf("z"));
```
A. 0  
B. -1  
C. 5  
D. Error  

---

### **14.** What is printed?
```java
String s = "ABCDE";
System.out.println(s.toLowerCase().substring(1, 4));
```
A. "bcd"  
B. "BCD"  
C. "bcde"  
D. "cde"  

---

### **15.** What is printed?
```java
double x = Math.random();
System.out.println(x >= 0 && x < 1);
```
A. true  
B. false  
C. Sometimes true  
D. Error  

---

# 🟧 **UNIT 2 PRACTICE SET B — FRQ‑STYLE TASKS**

### **FRQ 1 — Count Vowels**
Write a method that returns the number of vowels in a `String`.

```java
public static int countVowels(String s)
```

Example:  
`countVowels("banana")` → `3`

---

### **FRQ 2 — First Match**
Write a method that returns the **first index** where `target` appears in `text`.  
Use only `String` methods from the Quick Reference.

```java
public static int firstMatch(String text, String target)
```

Return `-1` if not found.

---

### **FRQ 3 — Random Password**
Write a method that returns a random 4‑letter lowercase password.

```java
public static String randomPassword()
```

Example output: `"xqmv"`

---

# 🟪 **UNIT 2 PRACTICE SET C — CODING DRILLS**

### **Drill 1 — Fill in the blank**
```java
String s = "hello";
char last = s.charAt(s._____ - 1);
```

---

### **Drill 2 — Predict the output**
```java
System.out.println("abc".substring(0, 0));
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

### **Drill 4 — Rewrite using compareTo**
Rewrite this using `compareTo`:
```java
if (a.equals(b)) { }
```

---

### **Drill 5 — Random range**
Generate a random integer from **5 to 10 inclusive**.

---

# 🟫 **ANSWER KEY (MCQ)**  
1. B  
2. B  
3. A  
4. B  
5. A  
6. B  
7. B  
8. B  
9. B  
10. A  
11. B  
12. A  
13. B  
14. A  
15. A  

---

# ✅ **PACKET 3 COMPLETE**

If you'd like, I can now generate:

### **Packet 4 — Unit 3: Boolean Expressions & If Statements (Checklist + MCQ + FRQ + Drills)**

Just say: **Generate Packet 4.**
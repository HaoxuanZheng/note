Here it is — **Packet 8** in clean, printable **Markdown**, matching the structure of Packets 1–7.

---

# 📘 **PACKET 8 — UNIT 7: ARRAYLIST**  
**Checklist + MCQ Set + FRQ Set + Coding Drills**  
**Print‑Ready Markdown**

---

# 🟦 **UNIT 7 CHECKLIST — ARRAYLIST**

## ✅ **1. Concepts**
- [ ] Difference between **array** and **ArrayList**  
- [ ] ArrayList is **resizable**, array is **fixed size**  
- [ ] ArrayList stores **objects**, not primitives (`Integer` instead of `int`)  
- [ ] Index‑based access  
- [ ] Methods from the **Java Quick Reference**:  
  - `add(obj)`  
  - `add(index, obj)`  
  - `get(index)`  
  - `set(index, obj)`  
  - `remove(index)`  
  - `size()`  
- [ ] Traversal using index loop  
- [ ] Safe removal while iterating  
- [ ] Enhanced for‑loop is **not safe** for removal  
- [ ] Common patterns: filter, transform, search  

---

## ✅ **2. Must‑Know Syntax**

### **Declaration**
```java
ArrayList<String> list = new ArrayList<String>();
ArrayList<Integer> nums = new ArrayList<Integer>();
```

### **Adding elements**
```java
list.add("A");
list.add(1, "B"); // insert at index 1
```

### **Accessing elements**
```java
String x = list.get(0);
```

### **Modifying elements**
```java
list.set(2, "Z");
```

### **Removing elements**
```java
list.remove(1); // removes element at index 1
```

### **Traversal**
```java
for (int i = 0; i < list.size(); i++) {
    System.out.println(list.get(i));
}
```

### **Safe removal**
```java
for (int i = 0; i < list.size(); i++) {
    if (condition) {
        list.remove(i);
        i--;
    }
}
```

---

## ✅ **3. Common Mistakes**
- [ ] Using `int` instead of `Integer`  
- [ ] Using enhanced for‑loop while removing elements  
- [ ] Forgetting that `size()` changes after removal  
- [ ] Confusing `set` and `add`  
- [ ] Using `<= list.size()` instead of `< list.size()`  
- [ ] Assuming `remove(obj)` is allowed — **AP CSA only uses `remove(index)`**  

---

## ✅ **4. Mini‑Patterns**

### **Filter pattern**
```java
for (int i = 0; i < list.size(); i++) {
    if (!condition) {
        list.remove(i);
        i--;
    }
}
```

### **Transform pattern**
```java
for (int i = 0; i < nums.size(); i++) {
    nums.set(i, nums.get(i) * 2);
}
```

### **Search pattern**
```java
for (int i = 0; i < list.size(); i++) {
    if (list.get(i).equals(target)) return i;
}
return -1;
```

---

# 🟩 **UNIT 7 PRACTICE SET A — MCQ (15 QUESTIONS)**  
*(Answer key at bottom)*

### **1.** What is printed?
```java
ArrayList<String> a = new ArrayList<String>();
a.add("hi");
System.out.println(a.get(0));
```
A. hi  
B. 0  
C. null  
D. Error  

---

### **2.** What is printed?
```java
ArrayList<Integer> a = new ArrayList<Integer>();
a.add(3);
a.add(7);
System.out.println(a.size());
```
A. 1  
B. 2  
C. 3  
D. Error  

---

### **3.** What is printed?
```java
ArrayList<Integer> a = new ArrayList<Integer>();
a.add(5);
a.add(1);
a.set(0, 9);
System.out.println(a.get(0));
```
A. 5  
B. 1  
C. 9  
D. Error  

---

### **4.** What is printed?
```java
ArrayList<String> a = new ArrayList<String>();
a.add("A");
a.add("B");
a.add(1, "C");
System.out.println(a);
```
A. [A, B, C]  
B. [A, C, B]  
C. [C, A, B]  
D. Error  

---

### **5.** What is printed?
```java
ArrayList<Integer> a = new ArrayList<Integer>();
a.add(2);
a.add(4);
a.add(6);
a.remove(1);
System.out.println(a.get(1));
```
A. 2  
B. 4  
C. 6  
D. Error  

---

### **6.** What is printed?
```java
ArrayList<String> a = new ArrayList<String>();
a.add("x");
a.add("y");
a.add("z");
for (int i = 0; i < a.size(); i++) {
    System.out.print(a.get(i));
}
```
A. xyz  
B. x y z  
C. xz  
D. Error  

---

### **7.** What is printed?
```java
ArrayList<Integer> a = new ArrayList<Integer>();
a.add(1);
a.add(2);
a.add(3);
for (int x : a) {
    System.out.print(x * 2 + " ");
}
```
A. 1 2 3  
B. 2 4 6  
C. 1 4 9  
D. Error  

---

### **8.** What is printed?
```java
ArrayList<Integer> a = new ArrayList<Integer>();
a.add(10);
a.add(20);
a.add(30);
System.out.println(a.get(a.size() - 1));
```
A. 10  
B. 20  
C. 30  
D. Error  

---

### **9.** What is printed?
```java
ArrayList<String> a = new ArrayList<String>();
a.add("a");
a.add("b");
a.add("c");
a.remove(0);
System.out.println(a.get(0));
```
A. a  
B. b  
C. c  
D. Error  

---

### **10.** What is printed?
```java
ArrayList<Integer> a = new ArrayList<Integer>();
a.add(1);
a.add(2);
a.add(3);
for (int i = 0; i < a.size(); i++) {
    a.set(i, a.get(i) + 1);
}
System.out.println(a.get(2));
```
A. 3  
B. 4  
C. 5  
D. Error  

---

### **11.** What is printed?
```java
ArrayList<Integer> a = new ArrayList<Integer>();
a.add(5);
a.add(5);
a.add(5);
int count = 0;
for (int i = 0; i < a.size(); i++) {
    if (a.get(i) == 5) count++;
}
System.out.println(count);
```
A. 0  
B. 1  
C. 2  
D. 3  

---

### **12.** What is printed?
```java
ArrayList<Integer> a = new ArrayList<Integer>();
a.add(1);
a.add(2);
a.add(3);
System.out.println(a.indexOf(2));
```
A. 0  
B. 1  
C. 2  
D. -1  

---

### **13.** What is printed?
```java
ArrayList<String> a = new ArrayList<String>();
a.add("hi");
a.add("bye");
System.out.println(a.remove(1));
```
A. hi  
B. bye  
C. 1  
D. Error  

---

### **14.** What is printed?
```java
ArrayList<Integer> a = new ArrayList<Integer>();
a.add(2);
a.add(4);
a.add(6);
for (int i = 0; i < a.size(); i++) {
    if (a.get(i) % 4 == 0) {
        a.remove(i);
        i--;
    }
}
System.out.println(a.size());
```
A. 1  
B. 2  
C. 3  
D. 0  

---

### **15.** What is printed?
```java
ArrayList<Integer> a = new ArrayList<Integer>();
a.add(1);
a.add(2);
a.add(3);
for (int x : a) {
    x = x * 10;
}
System.out.println(a.get(0));
```
A. 1  
B. 10  
C. 0  
D. Error  

---

# 🟧 **UNIT 7 PRACTICE SET B — FRQ‑STYLE TASKS**

### **FRQ 1 — Remove Short Words**
Remove all strings of length < 3 from an ArrayList.

```java
public static void removeShort(ArrayList<String> words)
```

---

### **FRQ 2 — Double All**
Multiply every element in an `ArrayList<Integer>` by 2.

```java
public static void doubleAll(ArrayList<Integer> nums)
```

---

### **FRQ 3 — Count Matches**
Count how many times `target` appears in an ArrayList.

```java
public static int countMatches(ArrayList<String> list, String target)
```

---

# 🟪 **UNIT 7 PRACTICE SET C — CODING DRILLS**

### **Drill 1 — Fill in the blank**
```java
list._____(index, value);   // replace element
```

---

### **Drill 2 — Predict the output**
```java
ArrayList<String> a = new ArrayList<String>();
a.add("x");
a.add("y");
a.add("z");
a.remove(1);
System.out.println(a);
```

---

### **Drill 3 — Fix the bug**
```java
ArrayList<int> nums = new ArrayList<int>();   // fix this
```

---

### **Drill 4 — Write a loop**
Print all elements **in reverse order**.

---

### **Drill 5 — Safe removal**
Remove all negative numbers from an `ArrayList<Integer>`.

---

# 🟫 **ANSWER KEY (MCQ)**  
1. A  
2. B  
3. C  
4. B  
5. C  
6. A  
7. B  
8. C  
9. B  
10. B  
11. D  
12. B  
13. B  
14. B  
15. A  

---

# ✅ **PACKET 8 COMPLETE**

If you'd like, I can now generate:

### **Packet 9 — Unit 8: 2D Arrays (Checklist + MCQ + FRQ + Drills)**

Just say: **Generate Packet 9.**
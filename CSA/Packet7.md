Here it is — **Packet 7** in clean, printable **Markdown**, matching the structure of Packets 1–6.

---

# 📘 **PACKET 7 — UNIT 6: ARRAYS**  
**Checklist + MCQ Set + FRQ Set + Coding Drills**  
**Print‑Ready Markdown**

---

# 🟦 **UNIT 6 CHECKLIST — ARRAYS**

## ✅ **1. Concepts**
- [ ] Array declaration and initialization  
- [ ] Fixed size (cannot grow or shrink)  
- [ ] Indexing: `0` to `length - 1`  
- [ ] Accessing and modifying elements  
- [ ] Traversal with loops  
- [ ] Enhanced for‑loop (read‑only)  
- [ ] Common array algorithms:  
  - Sum  
  - Count  
  - Max/min  
  - Linear search  
  - Copying arrays  
- [ ] Off‑by‑one errors  
- [ ] Difference between `length` (array) and `size()` (ArrayList)  

---

## ✅ **2. Must‑Know Syntax**

### **Declaration**
```java
int[] nums = new int[5];
String[] words = new String[10];
```

### **Initialization**
```java
int[] data = {3, 1, 4, 1, 5};
```

### **Traversal**
```java
for (int i = 0; i < data.length; i++) {
    System.out.println(data[i]);
}
```

### **Enhanced for‑loop**
```java
for (int value : data) {
    System.out.println(value);
}
```

*(Note: cannot modify array structure with enhanced for‑loop.)*

---

## ✅ **3. Common Mistakes**
- [ ] Using `<= data.length` instead of `< data.length`  
- [ ] Confusing `length` (array) with `length()` (String)  
- [ ] Forgetting arrays are fixed size  
- [ ] Using enhanced for‑loop when index is needed  
- [ ] Accessing uninitialized elements (default values: `0`, `false`, `null`)  

---

## ✅ **4. Mini‑Patterns**

### **Find max**
```java
int max = arr[0];
for (int i = 1; i < arr.length; i++) {
    if (arr[i] > max) max = arr[i];
}
```

### **Count matches**
```java
int count = 0;
for (int x : arr) {
    if (x % 2 == 0) count++;
}
```

### **Linear search**
```java
for (int i = 0; i < arr.length; i++) {
    if (arr[i] == target) return i;
}
return -1;
```

---

# 🟩 **UNIT 6 PRACTICE SET A — MCQ (15 QUESTIONS)**  
*(Answer key at bottom)*

### **1.** What is printed?
```java
int[] a = {2, 4, 6};
System.out.println(a[1]);
```
A. 2  
B. 4  
C. 6  
D. Error  

---

### **2.** What is printed?
```java
int[] a = new int[3];
System.out.println(a[2]);
```
A. 0  
B. null  
C. Error  
D. Garbage value  

---

### **3.** What is printed?
```java
int[] a = {1, 2, 3, 4};
System.out.println(a.length);
```
A. 3  
B. 4  
C. 5  
D. Error  

---

### **4.** What is printed?
```java
int[] a = {3, 1, 4};
a[1] = a[2];
System.out.println(a[1]);
```
A. 1  
B. 3  
C. 4  
D. Error  

---

### **5.** What is printed?
```java
int[] a = {1, 2, 3};
for (int i = 0; i < a.length; i++) {
    a[i] = a[i] * 2;
}
System.out.println(a[2]);
```
A. 3  
B. 4  
C. 6  
D. 8  

---

### **6.** What is printed?
```java
int[] a = {5, 4, 3, 2, 1};
int sum = 0;
for (int x : a) sum += x;
System.out.println(sum);
```
A. 10  
B. 12  
C. 15  
D. 20  

---

### **7.** What is printed?
```java
int[] a = {1, 3, 5, 7};
System.out.println(a[a.length - 1]);
```
A. 1  
B. 3  
C. 5  
D. 7  

---

### **8.** What is printed?
```java
int[] a = {2, 4, 6, 8};
for (int i = 1; i < a.length; i += 2) {
    System.out.print(a[i] + " ");
}
```
A. `2 6`  
B. `4 8`  
C. `4 6`  
D. `2 4`  

---

### **9.** What is printed?
```java
int[] a = {1, 2, 3};
System.out.println(a[3]);
```
A. 3  
B. Error  
C. 0  
D. null  

---

### **10.** What is printed?
```java
int[] a = {3, 3, 3};
int count = 0;
for (int i = 0; i < a.length; i++) {
    if (a[i] == 3) count++;
}
System.out.println(count);
```
A. 0  
B. 1  
C. 2  
D. 3  

---

### **11.** What is printed?
```java
int[] a = {4, 1, 2};
int max = a[0];
for (int i = 1; i < a.length; i++) {
    if (a[i] > max) max = a[i];
}
System.out.println(max);
```
A. 1  
B. 2  
C. 4  
D. 5  

---

### **12.** What is printed?
```java
int[] a = new int[4];
System.out.println(a.length);
```
A. 0  
B. 3  
C. 4  
D. Error  

---

### **13.** What is printed?
```java
int[] a = {1, 2, 3, 4};
for (int i = 0; i < a.length - 1; i++) {
    System.out.print(a[i]);
}
```
A. `1234`  
B. `123`  
C. `234`  
D. `12`  

---

### **14.** What is printed?
```java
int[] a = {2, 4, 6};
int i = 0;
while (i < a.length) {
    System.out.print(a[i]);
    i++;
}
```
A. `246`  
B. `24`  
C. `46`  
D. `26`  

---

### **15.** What is printed?
```java
int[] a = {1, 2, 3};
for (int x : a) {
    x = x * 10;
}
System.out.println(a[0]);
```
A. 1  
B. 10  
C. 0  
D. Error  

---

# 🟧 **UNIT 6 PRACTICE SET B — FRQ‑STYLE TASKS**

### **FRQ 1 — Count Negatives**
Write a method that returns the number of negative values in an `int[]`.

```java
public static int countNegatives(int[] arr)
```

---

### **FRQ 2 — Index of Max**
Return the **index** of the largest value in an array.  
If the array is empty, return `-1`.

```java
public static int indexOfMax(int[] arr)
```

---

### **FRQ 3 — All Even**
Return `true` if **all** elements in an array are even.

```java
public static boolean allEven(int[] arr)
```

---

# 🟪 **UNIT 6 PRACTICE SET C — CODING DRILLS**

### **Drill 1 — Fill in the blank**
```java
int last = arr[arr.______ - 1];
```

---

### **Drill 2 — Predict the output**
```java
int[] a = {1, 2, 3};
System.out.println(a.length);
```

---

### **Drill 3 — Fix the bug**
```java
int[] a = new int[5];
a[5] = 10;   // fix this
```

---

### **Drill 4 — Write a loop**
Print all **odd** values in an array.

---

### **Drill 5 — Reverse copy**
Write code to create a **new array** that is the reverse of `arr`.

---

# 🟫 **ANSWER KEY (MCQ)**  
1. B  
2. A  
3. B  
4. C  
5. C  
6. C  
7. D  
8. B  
9. B  
10. D  
11. C  
12. C  
13. B  
14. A  
15. A  

---

# ✅ **PACKET 7 COMPLETE**

If you'd like, I can now generate:

### **Packet 8 — Unit 7: ArrayList (Checklist + MCQ + FRQ + Drills)**

Just say: **Generate Packet 8.**
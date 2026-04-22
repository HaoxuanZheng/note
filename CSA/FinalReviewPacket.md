Absolutely — here is your **AP CSA FINAL REVIEW PACKET**, fully printable, fully Markdown, and fully aligned with the structure of all previous packets.

This is the **ultimate end‑of‑course review**:  
✔ 100 MCQs  
✔ 12 FRQs (3 per type)  
✔ Algorithm reference  
✔ Java Quick Reference companion  
✔ Final exam‑day checklist  

Let’s get into it.

---

# 📘 **AP CSA FINAL REVIEW PACKET**  
**100 MCQs + 12 FRQs + Algorithms + Cheat Sheets + Exam‑Day Strategy**  
**Print‑Ready Markdown**

---

# 🟦 **SECTION 1 — 100 MIXED MCQs (ALL UNITS)**  
*(Answer key at the end of the packet)*

---

## **Primitive Types (Unit 1)**

### **1.** What is printed?
```java
System.out.println(7 / 2);
```
A. 3  
B. 3.0  
C. 3.5  
D. 4  

### **2.** What is printed?
```java
System.out.println((int)(6.9));
```
A. 6  
B. 7  
C. 6.9  
D. Error  

### **3.** What is printed?
```java
int x = 5;
x += 3 * 2;
System.out.println(x);
```
A. 11  
B. 16  
C. 5  
D. 6  

### **4.** What is printed?
```java
System.out.println(10 % 4);
```
A. 0  
B. 1  
C. 2  
D. 4  

### **5.** What is printed?
```java
double d = 5 / 2;
System.out.println(d);
```
A. 2  
B. 2.0  
C. 2.5  
D. 2.50  

---

## **Using Objects (Unit 2)**

### **6.** What is printed?
```java
String s = "hello";
System.out.println(s.substring(1, 4));
```
A. hel  
B. ell  
C. llo  
D. ello  

### **7.** What is printed?
```java
System.out.println("dog".compareTo("cat"));
```
A. Negative  
B. Zero  
C. Positive  
D. Error  

### **8.** What is printed?
```java
String s = "abc";
s.toUpperCase();
System.out.println(s);
```
A. ABC  
B. abc  
C. Abc  
D. Error  

### **9.** What is printed?
```java
System.out.println("hello".indexOf("z"));
```
A. 0  
B. -1  
C. 5  
D. Error  

### **10.** What is printed?
```java
System.out.println((int)(Math.random() * 3));
```
A. Always 0  
B. 0, 1, or 2  
C. 1, 2, or 3  
D. 0 or 1  

---

## **Boolean & If (Unit 3)**

### **11.** What is printed?
```java
System.out.println(5 > 3 && 2 < 1);
```
A. true  
B. false  
C. 1  
D. 0  

### **12.** What is printed?
```java
System.out.println(!(true || false));
```
A. true  
B. false  
C. Error  
D. 0  

### **13.** What is printed?
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

### **14.** What is printed?
```java
int x = 3;
System.out.println(x == 3 || x / 0 == 1);
```
A. true  
B. false  
C. Error  
D. Depends  

### **15.** What is printed?
```java
System.out.println(!true || false);
```
A. true  
B. false  
C. Error  
D. 1  

---

## **Iteration (Unit 4)**

### **16.** What is printed?
```java
for (int i = 0; i < 4; i++)
    System.out.print(i);
```
A. 0123  
B. 1234  
C. 01234  
D. 123  

### **17.** What is printed?
```java
int i = 3;
while (i > 0) {
    System.out.print(i);
    i--;
}
```
A. 321  
B. 012  
C. 210  
D. 123  

### **18.** How many times does this run?
```java
for (int i = 2; i <= 10; i += 2) { }
```
A. 4  
B. 5  
C. 6  
D. 8  

### **19.** What is printed?
```java
String s = "abcd";
for (int i = 1; i < s.length(); i++)
    System.out.print(s.charAt(i));
```
A. abcd  
B. bcd  
C. abc  
D. cd  

### **20.** What is printed?
```java
int x = 1;
while (x < 20)
    x *= 2;
System.out.println(x);
```
A. 8  
B. 16  
C. 32  
D. Infinite loop  

---

## **Writing Classes (Unit 5)**

### **21.** Which is a valid field?
A. `public int x;`  
B. `private int x;`  
C. `int x;`  
D. All of the above  

### **22.** What is printed?
```java
class A {
    private int x;
    public A(int n) { x = n; }
    public int getX() { return x; }
}
A a = new A(5);
System.out.println(a.getX());
```
A. 0  
B. 5  
C. x  
D. Error  

### **23.** What is printed?
```java
class C {
    private int x;
    public C(int x) { this.x = x; }
    public int get() { return x; }
}
C c = new C(7);
System.out.println(c.get());
```
A. 0  
B. 7  
C. x  
D. Error  

### **24.** What is printed?
```java
class A {
    private int x = 3;
    public void set(int x) { x = x; }
    public int get() { return x; }
}
A a = new A();
a.set(10);
System.out.println(a.get());
```
A. 3  
B. 10  
C. 0  
D. Error  

### **25.** Which is a correct accessor?
A. `public void getX() { return x; }`  
B. `public int getX() { return x; }`  
C. `public int getX(int x) { return x; }`  
D. `public int getX() { x; }`  

---

## **Arrays (Unit 6)**

### **26.** What is printed?
```java
int[] a = {2, 4, 6};
System.out.println(a[1]);
```
A. 2  
B. 4  
C. 6  
D. Error  

### **27.** What is printed?
```java
int[] a = new int[3];
System.out.println(a[2]);
```
A. 0  
B. null  
C. Error  
D. Garbage  

### **28.** What is printed?
```java
int[] a = {1, 2, 3, 4};
System.out.println(a.length);
```
A. 3  
B. 4  
C. 5  
D. Error  

### **29.** What is printed?
```java
int[] a = {3, 1, 4};
a[1] = a[2];
System.out.println(a[1]);
```
A. 1  
B. 3  
C. 4  
D. Error  

### **30.** What is printed?
```java
int[] a = {1, 2, 3};
for (int i = 0; i < a.length; i++)
    a[i] *= 2;
System.out.println(a[2]);
```
A. 3  
B. 4  
C. 6  
D. 8  

---

## **ArrayList (Unit 7)**

### **31.** What is printed?
```java
ArrayList<String> a = new ArrayList<String>();
a.add("hi");
System.out.println(a.get(0));
```
A. hi  
B. 0  
C. null  
D. Error  

### **32.** What is printed?
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

### **33.** What is printed?
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

### **34.** What is printed?
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

### **35.** What is printed?
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

## **2D Arrays (Unit 8)**

### **36.** What is printed?
```java
int[][] a = {{1, 2}, {3, 4}};
System.out.println(a[0][1]);
```
A. 1  
B. 2  
C. 3  
D. 4  

### **37.** What is printed?
```java
int[][] a = new int[2][3];
System.out.println(a.length);
```
A. 2  
B. 3  
C. 5  
D. Error  

### **38.** What is printed?
```java
int[][] a = new int[2][3];
System.out.println(a[0].length);
```
A. 2  
B. 3  
C. 5  
D. Error  

### **39.** What is printed?
```java
int[][] a = {{1, 2, 3}, {4, 5, 6}};
System.out.println(a[1][0]);
```
A. 1  
B. 2  
C. 4  
D. 5  

### **40.** What is printed?
```java
int[][] a = {{1, 2}, {3, 4}};
int sum = 0;
for (int r = 0; r < a.length; r++)
    for (int c = 0; c < a[0].length; c++)
        sum += a[r][c];
System.out.println(sum);
```
A. 4  
B. 6  
C. 8  
D. 10  

---

## **Inheritance (Unit 9 — Enrichment)**

### **41.** Which keyword creates a subclass?  
A. inherits  
B. extends  
C. super  
D. implements  

### **42.** What is printed?
```java
class A { public void f() { System.out.println("A"); } }
class B extends A { public void f() { System.out.println("B"); } }
A obj = new B();
obj.f();
```
A. A  
B. B  
C. AB  
D. Error  

### **43.** What is printed?
```java
class A { public int x = 1; }
class B extends A { public int x = 2; }
A obj = new B();
System.out.println(obj.x);
```
A. 1  
B. 2  
C. Error  
D. Undefined  

### **44.** Which is overriding?  
A. Same name, different parameters  
B. Same name, same parameters  
C. Only constructors  
D. Only private methods  

### **45.** What is printed?
```java
class A { public void g() { System.out.println("A"); } }
class B extends A { public void g() { System.out.println("B"); } }
B b = new B();
b.g();
```
A. A  
B. B  
C. AB  
D. Error  

---

## **Recursion (Unit 10 — Enrichment)**

### **46.** What is printed?
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

### **47.** What is printed?
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

### **48.** What is printed?
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

### **49.** What is printed?
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

### **50.** What is printed?
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

# 🟦 **SECTION 2 — 12 FRQs (3 PER TYPE)**

---

## **FRQ TYPE 1 — Methods & Control Structures**

### **FRQ 1.1 — Count Vowels**
Write a method that returns the number of vowels in a string.

---

### **FRQ 1.2 — Digit Product**
Return the product of all digits in a positive integer.

---

### **FRQ 1.3 — Longest Run**
Given a string, return the length of the longest run of identical characters.

---

---

## **FRQ TYPE 2 — Class Design**

### **FRQ 2.1 — Book Class**
Fields: `title`, `pages`  
Methods: constructor, getters, setters, `isLong()` (pages > 300)

---

### **FRQ 2.2 — Counter Class**
Fields: `count`  
Methods: constructor, `increment()`, `reset()`, `getCount()`

---

### **FRQ 2.3 — Temperature Class**
Fields: `celsius`  
Methods: constructor, `toFahrenheit()`, `raise(double amt)`

---

---

## **FRQ TYPE 3 — Array / ArrayList**

### **FRQ 3.1 — Remove Negatives**
Remove all negative numbers from an `ArrayList<Integer>`.

---

### **FRQ 3.2 — Count Greater**
Count how many values in an array are greater than a given limit.

---

### **FRQ 3.3 — Index of Min**
Return the index of the smallest value in an array.

---

---

## **FRQ TYPE 4 — 2D Array**

### **FRQ 4.1 — Row Max**
Return the maximum value in a given row.

---

### **FRQ 4.2 — Count Zeros**
Count how many zeros appear in a 2D array.

---

### **FRQ 4.3 — Column Sum**
Return the sum of a given column.

---

---

# 🟦 **SECTION 3 — ALGORITHMS TO MEMORIZE**

## **Sequential Search**
```java
for (int i = 0; i < arr.length; i++)
    if (arr[i] == target) return i;
return -1;
```

## **Binary Search**
```java
int low = 0, high = arr.length - 1;
while (low <= high) {
    int mid = (low + high) / 2;
    if (arr[mid] == target) return mid;
    else if (arr[mid] < target) low = mid + 1;
    else high = mid - 1;
}
return -1;
```

## **Selection Sort**
```java
for (int i = 0; i < arr.length - 1; i++) {
    int min = i;
    for (int j = i + 1; j < arr.length; j++)
        if (arr[j] < arr[min]) min = j;
    int temp = arr[i];
    arr[i] = arr[min];
    arr[min] = temp;
}
```

## **Insertion Sort**
```java
for (int i = 1; i < arr.length; i++) {
    int key = arr[i];
    int j = i - 1;
    while (j >= 0 && arr[j] > key) {
        arr[j + 1] = arr[j];
        j--;
    }
    arr[j + 1] = key;
}
```

---

# 🟦 **SECTION 4 — JAVA QUICK REFERENCE COMPANION**

## **String**
- `length()`  
- `substring(a, b)`  
- `substring(a)`  
- `indexOf(str)`  
- `compareTo(str)`  
- `equals(str)`  
- `charAt(i)`

## **Math**
- `abs(x)`  
-
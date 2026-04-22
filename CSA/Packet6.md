Here it is — **Packet 6** in clean, printable **Markdown**, matching the structure of Packets 1–5.

---

# 📘 **PACKET 6 — UNIT 5: WRITING CLASSES**  
**Checklist + MCQ Set + FRQ Set + Coding Drills**  
**Print‑Ready Markdown**

---

# 🟦 **UNIT 5 CHECKLIST — WRITING CLASSES**

## ✅ **1. Concepts**
- [ ] What a **class** is (blueprint for objects)  
- [ ] Fields (instance variables)  
- [ ] Constructors (default + parameterized)  
- [ ] Accessor methods (getters)  
- [ ] Mutator methods (setters)  
- [ ] `this` keyword  
- [ ] Encapsulation (`private` fields, `public` methods)  
- [ ] Method overloading (same name, different parameters)  
- [ ] Object state changes  
- [ ] No static fields unless specified  

---

## ✅ **2. Must‑Know Syntax**

### **Class structure**
```java
public class Person {
    private String name;
    private int age;

    public Person(String n, int a) {
        name = n;
        age = a;
    }

    public String getName() { return name; }
    public int getAge() { return age; }

    public void setAge(int a) { age = a; }
}
```

### **Using `this`**
```java
public Person(String name, int age) {
    this.name = name;
    this.age = age;
}
```

### **Mutator pattern**
```java
public void setValue(int v) {
    value = v;
}
```

### **Accessor pattern**
```java
public int getValue() {
    return value;
}
```

---

## ✅ **3. Common Mistakes**
- [ ] Forgetting to initialize fields in constructor  
- [ ] Using local variables instead of fields  
- [ ] Returning wrong type in accessor  
- [ ] Mutator not updating the field  
- [ ] Missing `this` when parameter names shadow fields  
- [ ] Adding extra fields not in the specification  
- [ ] Forgetting `private` on fields  

---

## ✅ **4. Mini‑Patterns**

### **Constructor with validation**
```java
public BankAccount(double initial) {
    if (initial < 0) balance = 0;
    else balance = initial;
}
```

### **Incrementing a field**
```java
public void deposit(double amt) {
    balance += amt;
}
```

### **Boolean method**
```java
public boolean isAdult() {
    return age >= 18;
}
```

---

# 🟩 **UNIT 5 PRACTICE SET A — MCQ (15 QUESTIONS)**  
*(Answer key at bottom)*

### **1.** Which is a valid field declaration?
A. `public int x;`  
B. `private int x;`  
C. `int x;`  
D. All of the above  

---

### **2.** What is printed?
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

---

### **3.** What is printed?
```java
class Counter {
    private int c = 0;
    public void inc() { c++; }
    public int get() { return c; }
}

Counter ct = new Counter();
ct.inc();
ct.inc();
System.out.println(ct.get());
```
A. 0  
B. 1  
C. 2  
D. Error  

---

### **4.** What is wrong with this class?
```java
class Box {
    public int size;
    public Box(int s) { size = s; }
}
```
A. Field should be private  
B. Constructor is wrong  
C. Missing return type  
D. Nothing  

---

### **5.** What is printed?
```java
class P {
    private int x;
    public P() { x = 10; }
    public P(int n) { x = n; }
    public int get() { return x; }
}

P p = new P();
System.out.println(p.get());
```
A. 0  
B. 10  
C. n  
D. Error  

---

### **6.** What is printed?
```java
class Dog {
    private String name;
    public Dog(String n) { name = n; }
    public void setName(String n) { name = n; }
    public String getName() { return name; }
}

Dog d = new Dog("Rex");
d.setName("Max");
System.out.println(d.getName());
```
A. Rex  
B. Max  
C. name  
D. Error  

---

### **7.** What is printed?
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

---

### **8.** What is printed?
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

---

### **9.** What is printed?
```java
class S {
    private String s;
    public S(String str) { s = str; }
    public String get() { return s; }
}

S obj = new S("hi");
System.out.println(obj);
```
A. hi  
B. S@something  
C. Error  
D. null  

---

### **10.** What is printed?
```java
class A {
    private int x;
    public A(int n) { x = n; }
    public void add(int n) { x += n; }
    public int get() { return x; }
}

A a = new A(5);
a.add(3);
System.out.println(a.get());
```
A. 3  
B. 5  
C. 8  
D. Error  

---

### **11.** Which is a correct accessor?
A. `public void getX() { return x; }`  
B. `public int getX() { return x; }`  
C. `public int getX(int x) { return x; }`  
D. `public int getX() { x; }`  

---

### **12.** Which is true?
```java
private int x;
```
A. Accessible everywhere  
B. Accessible only inside the class  
C. Accessible in subclasses  
D. Accessible in same package  

---

### **13.** What is printed?
```java
class A {
    private int x = 1;
    public A() { x = 2; }
    public A(int n) { x = n; }
    public int get() { return x; }
}

A a = new A(5);
System.out.println(a.get());
```
A. 1  
B. 2  
C. 5  
D. Error  

---

### **14.** What is printed?
```java
class A {
    private int x = 1;
    public A() { }
    public int get() { return x; }
}

A a = new A();
System.out.println(a.get());
```
A. 0  
B. 1  
C. null  
D. Error  

---

### **15.** What is printed?
```java
class A {
    private int x;
    public A(int n) { x = n; }
    public void set(int n) { x = n; }
    public int get() { return x; }
}

A a = new A(4);
a.set(a.get() + 6);
System.out.println(a.get());
```
A. 4  
B. 6  
C. 10  
D. Error  

---

# 🟧 **UNIT 5 PRACTICE SET B — FRQ‑STYLE TASKS**

### **FRQ 1 — Simple BankAccount**
Write a class `BankAccount` with:
- A private `double balance`  
- A constructor `BankAccount(double initial)`  
- A method `deposit(double amt)`  
- A method `withdraw(double amt)` (only if enough balance)  
- A method `getBalance()`  

---

### **FRQ 2 — Student Class**
Write a class `Student` with:
- Fields: `name` (String), `grade` (int)  
- Constructor: `Student(String n, int g)`  
- Accessors for both fields  
- Mutator for grade  
- Method `isPassing()` (grade ≥ 65)  

---

### **FRQ 3 — Rectangle**
Write a class `Rectangle` with:
- Fields: `width`, `height`  
- Constructor  
- `getArea()`  
- `getPerimeter()`  
- `isSquare()`  

---

# 🟪 **UNIT 5 PRACTICE SET C — CODING DRILLS**

### **Drill 1 — Fill in the blank**
```java
private int score;
public int getScore() {
    return ______;
}
```

---

### **Drill 2 — Predict the output**
```java
class A {
    private int x = 5;
    public void set(int x) { this.x = x; }
    public int get() { return x; }
}

A a = new A();
a.set(12);
System.out.println(a.get());
```

---

### **Drill 3 — Fix the bug**
```java
public void setName(String name) {
    name = name;   // fix this
}
```

---

### **Drill 4 — Write a constructor**
Write a constructor for:
```java
private String title;
private int pages;
```

---

### **Drill 5 — Add a method**
Add a method to increase `pages` by 10.

---

# 🟫 **ANSWER KEY (MCQ)**  
1. D  
2. B  
3. C  
4. A  
5. B  
6. B  
7. B  
8. A  
9. B  
10. C  
11. B  
12. B  
13. C  
14. B  
15. C  

---

# ✅ **PACKET 6 COMPLETE**

If you'd like, I can now generate:

### **Packet 7 — Unit 6: Arrays (Checklist + MCQ + FRQ + Drills)**

Just say: **Generate Packet 7.**
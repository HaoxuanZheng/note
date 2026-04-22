Here it is — **Packet 10** in clean, printable **Markdown**, matching the structure of Packets 1–9.

> **Note:** Inheritance is *enrichment* in the new AP CSA CED (2025–26), but many teachers still teach it, and it remains excellent preparation for college‑level CS. This packet keeps it concise and AP‑aligned.

---

# 📘 **PACKET 10 — UNIT 9: INHERITANCE (ENRICHMENT)**  
**Checklist + MCQ Set + FRQ Set + Coding Drills**  
**Print‑Ready Markdown**

---

# 🟦 **UNIT 9 CHECKLIST — INHERITANCE**

## ✅ **1. Concepts**
- [ ] Purpose of inheritance (code reuse, specialization)  
- [ ] `extends` keyword  
- [ ] Superclass vs. subclass  
- [ ] Method overriding  
- [ ] Using `super()` to call superclass constructor  
- [ ] Polymorphism basics (compile‑time type vs. run‑time type)  
- [ ] Overriding vs. overloading  
- [ ] Access modifiers (`public`, `private`, `protected`)  
- [ ] What *is* and *is not* inherited  
- [ ] When to use `super.methodName()`  

---

## ✅ **2. Must‑Know Syntax**

### **Basic inheritance**
```java
public class Animal {
    public void speak() {
        System.out.println("...");
    }
}

public class Dog extends Animal {
    @Override
    public void speak() {
        System.out.println("Woof");
    }
}
```

### **Calling superclass constructor**
```java
public class Student extends Person {
    public Student(String name, int id) {
        super(name);   // call Person constructor
        this.id = id;
    }
}
```

### **Polymorphism**
```java
Animal a = new Dog();   // reference type Animal, object type Dog
a.speak();              // calls Dog's speak()
```

---

## ✅ **3. Common Mistakes**
- [ ] Forgetting `extends`  
- [ ] Forgetting `@Override` (not required but recommended)  
- [ ] Trying to override a `private` method (not allowed)  
- [ ] Confusing overriding with overloading  
- [ ] Forgetting to call `super(...)` when needed  
- [ ] Assuming fields are overridden (only methods can be overridden)  
- [ ] Misunderstanding reference type vs. object type  

---

## ✅ **4. Mini‑Patterns**

### **Override pattern**
```java
@Override
public void methodName() {
    // new behavior
}
```

### **Subclass constructor**
```java
public Sub(int x, int y) {
    super(x);   // call superclass constructor
    this.y = y;
}
```

### **Polymorphic call**
```java
Parent p = new Child();
p.doSomething();   // Child version runs
```

---

# 🟩 **UNIT 9 PRACTICE SET A — MCQ (15 QUESTIONS)**  
*(Answer key at bottom)*

### **1.** Which keyword is used to create a subclass?  
A. `inherits`  
B. `extends`  
C. `super`  
D. `implements`  

---

### **2.** What is printed?
```java
class A {
    public void f() { System.out.println("A"); }
}
class B extends A {
    public void f() { System.out.println("B"); }
}

A obj = new B();
obj.f();
```
A. A  
B. B  
C. AB  
D. Error  

---

### **3.** What is printed?
```java
class A {
    public int x = 1;
}
class B extends A {
    public int x = 2;
}

A obj = new B();
System.out.println(obj.x);
```
A. 1  
B. 2  
C. Error  
D. Undefined  

---

### **4.** Which is true about overriding?  
A. Same name, different parameters  
B. Same name, same parameters  
C. Only constructors can be overridden  
D. Only private methods can be overridden  

---

### **5.** What is printed?
```java
class A {
    public void g() { System.out.println("A"); }
}
class B extends A {
    public void g() { System.out.println("B"); }
}

B b = new B();
b.g();
```
A. A  
B. B  
C. AB  
D. Error  

---

### **6.** What is printed?
```java
class A {
    public void h() { System.out.println("A"); }
}
class B extends A {
}

B b = new B();
b.h();
```
A. A  
B. B  
C. Error  
D. Nothing  

---

### **7.** What is printed?
```java
class A {
    public void f() { System.out.println("A"); }
}
class B extends A {
    public void f() { System.out.println("B"); }
}
class C extends B {
    public void f() { System.out.println("C"); }
}

A obj = new C();
obj.f();
```
A. A  
B. B  
C. C  
D. Error  

---

### **8.** Which is true?  
```java
class A {}
class B extends A {}
```
A. B is a subclass of A  
B. A is a subclass of B  
C. A and B are unrelated  
D. B inherits from Object but not A  

---

### **9.** What is printed?
```java
class A {
    public void f() { System.out.println("A"); }
}
class B extends A {
    public void f() { System.out.println("B"); }
}

A a = new A();
B b = new B();
a = b;
a.f();
```
A. A  
B. B  
C. AB  
D. Error  

---

### **10.** What is printed?
```java
class A {
    public void f() { System.out.println("A"); }
}
class B extends A {
    public void g() { System.out.println("G"); }
}

A obj = new B();
obj.g();
```
A. G  
B. A  
C. Error  
D. Nothing  

---

### **11.** What is printed?
```java
class A {
    public A() { System.out.println("A"); }
}
class B extends A {
    public B() { System.out.println("B"); }
}

B b = new B();
```
A. A  
B. B  
C. AB  
D. BA  

---

### **12.** Which is true about constructors?  
A. Constructors are inherited  
B. Constructors are not inherited  
C. Constructors can be overridden  
D. Constructors must be private  

---

### **13.** What is printed?
```java
class A {
    public void f() { System.out.println("A"); }
}
class B extends A {
    public void f(int x) { System.out.println("B"); }
}

B b = new B();
b.f();
```
A. A  
B. B  
C. Error  
D. Nothing  

---

### **14.** What is printed?
```java
class A {
    public int get() { return 1; }
}
class B extends A {
    public int get() { return 2; }
}

A obj = new B();
System.out.println(obj.get());
```
A. 1  
B. 2  
C. Error  
D. Undefined  

---

### **15.** What is printed?
```java
class A {
    public void f() { System.out.println("A"); }
}
class B extends A {
    public void f() { System.out.println("B"); }
}
class C extends B {
}

C c = new C();
c.f();
```
A. A  
B. B  
C. C  
D. Error  

---

# 🟧 **UNIT 9 PRACTICE SET B — FRQ‑STYLE TASKS**

### **FRQ 1 — Shape Hierarchy**
Write two classes:

**Superclass:**  
```java
public class Shape {
    private String name;
    public Shape(String n) { name = n; }
    public String getName() { return name; }
    public double area() { return 0; }
}
```

**Subclass:**  
```java
public class Circle extends Shape {
    private double radius;
    public Circle(double r) { super("Circle"); radius = r; }
    @Override
    public double area() { return Math.PI * radius * radius; }
}
```

---

### **FRQ 2 — Employee / Manager**
Write:

**Employee**  
- Fields: `name`, `salary`  
- Methods: constructor, getters, `raise(double amt)`  

**Manager extends Employee**  
- Additional field: `department`  
- Override `toString()` to include department  

---

### **FRQ 3 — Animal Sounds**
Create:

**Animal** with method `speak()`  
**Dog extends Animal** overriding `speak()`  
**Cat extends Animal** overriding `speak()`  

---

# 🟪 **UNIT 9 PRACTICE SET C — CODING DRILLS**

### **Drill 1 — Fill in the blank**
```java
public class Dog ______ Animal { }
```

---

### **Drill 2 — Predict the output**
```java
A a = new B();
a.f();
```

---

### **Drill 3 — Fix the bug**
```java
class B extends A {
    public B() {
        name = "Bob";   // name is private in A
    }
}
```

---

### **Drill 4 — Write a constructor**
Subclass constructor that calls superclass constructor.

---

### **Drill 5 — Override a method**
Override `public String toString()` in a subclass.

---

# 🟫 **ANSWER KEY (MCQ)**  
1. B  
2. B  
3. A  
4. B  
5. B  
6. A  
7. C  
8. A  
9. B  
10. C  
11. C  
12. B  
13. A  
14. B  
15. B  

---

# ✅ **PACKET 10 COMPLETE**

If you'd like, I can now generate:

### **Packet 11 — Unit 10: Recursion (Checklist + MCQ + FRQ + Drills)**  
Just say: **Generate Packet 11.**
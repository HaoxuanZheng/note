# AP Computer Science A Ultimate Study Guide (2025–2026)

> Designed so you can realistically aim for a 5—with focus on what the *current* exam actually tests.

---

## 1. Exam overview

### Format and timing

| Section | Questions | Time | Weight | Mode |
|--------|-----------|------|--------|------|
| Section I | 42 MCQ | 90 min | 55% | Digital (Bluebook) |
| Section II | 4 FRQ | 90 min | 45% | Digital (Bluebook) |

- **MCQ:** Mostly standalone questions, some 2-question sets; 4 answer choices; no guessing penalty.  [AP Central](https://apcentral.collegeboard.org/courses/ap-computer-science-a/exam)  [skylit.com](https://skylit.com/beprepared/2025-CED-Sample-MC-Solutions.pdf)  
- **FRQ:** 4 fixed types, all in Java, with Java Quick Reference built into Bluebook.  [AP Central](https://apcentral.collegeboard.org/courses/ap-computer-science-a/exam)  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  

### FRQ question types (current spec)

- **Q1 – Methods & Control Structures:** Write 2 methods *or* 1 constructor + 1 method; heavy on `if`/loops and `String` use.  [AP Central](https://apcentral.collegeboard.org/courses/ap-computer-science-a/exam)  
- **Q2 – Class Design:** Design/implement a class from a spec table (header, fields, constructor, methods).  
- **Q3 – Data Analysis with ArrayList:** One method manipulating an `ArrayList`.  
- **Q4 – 2D Array:** One or more methods traversing and updating a 2D array.

### Scoring and 1–5 scale

- **MCQ:** Computer-scored; each correct = 1 raw point; no penalty for wrong/blank.  
- **FRQ:** Each question scored on a **0–9 rubric** (roughly 9 scoring rows: correctness, control structures, array/ArrayList use, etc.).  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  
- Raw MCQ + FRQ are combined and converted to a composite score; College Board then sets cut scores for 1–5 each year (not public, but historically: strong FRQ can compensate for some MCQ misses).

### 2025–2026 updates (important!)

- **New CED (effective Fall 2025):** Course reorganized into **4 big units**; **inheritance and polymorphism removed** from required content; recursion is de‑emphasized.  [apcsexamprep.com](https://www.apcsexamprep.com/pages/ap-csa-exam-prep-hub)  [skylit.com](https://skylit.com/beprepared/2025-CED-Sample-MC-Solutions.pdf)  
- **Exam remains:** 42 MCQ + 4 FRQ, fully digital, Java Quick Reference provided.  [AP Central](https://apcentral.collegeboard.org/courses/ap-computer-science-a/exam)  
- **What this means for you:**
  - Focus heavily on **objects, control structures, arrays, ArrayList, 2D arrays, algorithms**.
  - **Inheritance/recursion** are now enrichment topics—good for deeper understanding, but low/zero exam weight.

> I’ll still use the classic 10-unit structure you requested, but I’ll flag where content is now “enrichment”.

---

## 2. Unit‑by‑unit breakdown (classic 10 units)

For each unit:

- **Subtopics & objectives** (paraphrased from CED)  
- **Key syntax/patterns**  
- **Common exam questions**  
- **Frequent mistakes**  
- **Short annotated example**

---

### Unit 1 – Primitive types

#### Subtopics & learning goals

- **Data types:** `int`, `double`, `boolean`, `char`.  
- **Variables:** declaration, initialization, assignment, scope.  
- **Expressions:** arithmetic, integer vs. double division, casting.  
- **Constants:** `final` variables.  
- **Overflow and rounding** behavior.  [AP Students | College Board](https://apstudents.collegeboard.org/courses/ap-computer-science-a)  

#### Key syntax & patterns

- **Declaration/assignment:**
  ```java
  int count = 0;
  double price = 19.99;
  boolean done = false;
  char grade = 'A';
  ```
- **Integer vs. double division:**
  ```java
  int a = 5 / 2;      // 2
  double b = 5 / 2.0; // 2.5
  ```
- **Casting:**
  ```java
  double x = 7.9;
  int y = (int) x;    // 7
  ```

#### Common exam questions

- Evaluate expressions, especially **mixed int/double**.  
- Determine **result type** and value of expressions.  
- Identify **compile-time errors** (e.g., using uninitialized variables).

#### Frequent mistakes & fixes

- **Mistake:** Expecting `5 / 2` to be `2.5`.  
  - **Fix:** Remember: `int / int` → `int`. At least one operand must be `double`.  
- **Mistake:** Using variables before initialization.  
  - **Fix:** Always assign a value when you declare, especially in FRQs.  
- **Mistake:** Misunderstanding `%` (modulo).  
  - **Fix:** Practice with positive integers; know `% 10` gives last digit.

#### Example

```java
public class Discount {
    public static void main(String[] args) {
        double price = 19.99;
        int percentOff = 20;

        double discount = price * percentOff / 100.0; // 3.998
        double finalPrice = price - discount;         // 15.992

        System.out.println(finalPrice); // 15.992
    }
}
// Note: integer vs. double division matters in percent calculations.
```

---

### Unit 2 – Using objects

#### Subtopics & learning goals

- **Classes vs. objects:** instances, state, behavior.  
- **Constructors:** `new` keyword, parameters.  
- **Method calls:** return vs. `void`, parameters, side effects.  
- **`String` as a reference type.**  
- **APIs and libraries:** using provided classes (e.g., `Math`, `String`).  [AP Students | College Board](https://apstudents.collegeboard.org/courses/ap-computer-science-a)  

#### Key syntax & patterns

```java
String s = new String("hello"); // rarely used; usually:
String t = "hello";

int len = t.length();
String sub = t.substring(1, 4); // "ell"
int idx = t.indexOf("lo");      // 3

double r = Math.sqrt(25);       // 5.0
int m = Math.max(3, 7);         // 7
```

#### Common exam questions

- Predict output of code using **`String` methods**.  
- Determine **object state** after a sequence of method calls.  
- Use **APIs** correctly (e.g., `substring` indices).

#### Frequent mistakes & fixes

- **Mistake:** Off‑by‑one with `substring(begin, end)` (end is **exclusive**).  
- **Mistake:** Assuming `String` methods mutate the original string.  
  - All `String` methods return a **new** `String`; original is unchanged.  
- **Mistake:** Swapping parameter order in `Math` methods.

#### Example

```java
public class Greeting {
    public static void main(String[] args) {
        String name = "Haoxuan";
        String firstThree = name.substring(0, 3); // "Hao"
        int indexOfX = name.indexOf("x");         // 3

        System.out.println(firstThree + " " + indexOfX);
    }
}
// Shows substring and indexOf; both are heavily tested.
```

---

### Unit 3 – Boolean expressions and if statements

#### Subtopics & learning goals

- **Relational operators:** `==`, `!=`, `<`, `>`, `<=`, `>=`.  
- **Logical operators:** `&&`, `||`, `!` and **short‑circuit evaluation**.  
- **`if`, `if-else`, `if-else-if` chains.**  
- **De Morgan’s laws** and equivalent conditions.  [apcsexamprep.com](https://www.apcsexamprep.com/pages/ap-csa-exam-prep-hub)  

#### Key syntax & patterns

```java
if (score >= 90) {
    grade = 'A';
} else if (score >= 80) {
    grade = 'B';
} else {
    grade = 'C';
}

if (!(x > 0 && y > 0)) {
    // equivalent to: x <= 0 || y <= 0
}
```

#### Common exam questions

- Determine **branch taken** for given inputs.  
- Rewrite conditions using **De Morgan’s laws**.  
- Identify **unreachable branches** or logic errors.

#### Frequent mistakes & fixes

- **Mistake:** Using `==` to compare `String` objects.  
  - **Fix:** Use `str1.equals(str2)` instead.  
- **Mistake:** Misreading `&&` vs. `||`.  
- **Mistake:** Forgetting that `else` pairs with the **nearest** unmatched `if`.

#### Example

```java
public static boolean isValidPassword(String pwd) {
    // At least 8 chars and contains '@'
    return pwd.length() >= 8 && pwd.indexOf("@") != -1;
}
// Typical exam pattern: combine length and content checks with &&.
```

---

### Unit 4 – Iteration

#### Subtopics & learning goals

- **`while` loops** and **`for` loops**.  
- **Loop control variables**, initialization, update, termination.  
- **Nested loops** and counting patterns.  
- **String traversal with `charAt`.**  [apcsexamprep.com](https://www.apcsexamprep.com/pages/ap-csa-exam-prep-hub)  [Fiveable](https://fiveable.me/ap-comp-sci-a/ap-computer-science-a-exam/ap-comp-sci-a-ap-csa-mcq/study-guide/ap-comp-sci-a-ap-csa-mcq)  

#### Key syntax & patterns

```java
// for loop
for (int i = 0; i < n; i++) {
    // body
}

// while loop
int i = 0;
while (i < n) {
    // body
    i++;
}

// String traversal
for (int i = 0; i < s.length(); i++) {
    char c = s.charAt(i);
}
```

#### Common exam questions

- Trace loops and determine **final variable values** or **output**.  
- Count how many times a loop executes.  
- Identify **infinite loops** or off‑by‑one errors.

#### Frequent mistakes & fixes

- **Mistake:** Forgetting to update loop variable → infinite loop.  
- **Mistake:** Using `<= s.length()` instead of `< s.length()`.  
- **Mistake:** Modifying a collection incorrectly inside a loop.

#### Example

```java
public static int countVowels(String s) {
    int count = 0;
    String vowels = "aeiouAEIOU";
    for (int i = 0; i < s.length(); i++) {
        char c = s.charAt(i);
        if (vowels.indexOf(c) != -1) {
            count++;
        }
    }
    return count;
}
// Classic pattern: String traversal + indexOf.
```

---

### Unit 5 – Writing classes

> **Note:** Class design is still heavily tested; inheritance is not required in the new CED.  [apcsexamprep.com](https://www.apcsexamprep.com/pages/ap-csa-exam-prep-hub)  

#### Subtopics & learning goals

- **Class structure:** fields, constructors, methods.  
- **Encapsulation:** `private` fields, `public` methods.  
- **Accessors (getters) and mutators (setters).**  
- **`this` keyword** and constructor overloading.  

#### Key syntax & patterns

```java
public class Counter {
    private int value;

    public Counter() {
        value = 0;
    }

    public Counter(int start) {
        value = start;
    }

    public void increment() {
        value++;
    }

    public int getValue() {
        return value;
    }
}
```

#### Common exam questions

- Implement a class from a **spec table** (FRQ Q2 style).  
- Decide which fields/methods are needed.  
- Use **accessors/mutators** correctly.

#### Frequent mistakes & fixes

- **Mistake:** Forgetting to initialize fields in constructor.  
- **Mistake:** Using local variables instead of fields.  
- **Mistake:** Returning `void` where a value is required (or vice versa).

#### Example

```java
public class BankAccount {
    private String owner;
    private double balance;

    public BankAccount(String owner, double initial) {
        this.owner = owner;
        balance = initial;
    }

    public void deposit(double amount) {
        balance += amount;
    }

    public double getBalance() {
        return balance;
    }
}
// This is exactly the style of many Class FRQs.
```

---

### Unit 6 – Array

#### Subtopics & learning goals

- **Declare, create, and initialize arrays.**  
- **Indexing and bounds:** `0` to `length - 1`.  
- **Traversal patterns:** forward, backward, conditional.  
- **Common algorithms:** sum, count, max/min, search.  [apcsexamprep.com](https://www.apcsexamprep.com/pages/ap-csa-exam-prep-hub)  

#### Key syntax & patterns

```java
int[] nums = new int[5];
int[] data = {3, 1, 4, 1, 5};

for (int i = 0; i < data.length; i++) {
    System.out.println(data[i]);
}
```

#### Common exam questions

- Trace array algorithms.  
- Implement **search** or **count** logic.  
- Modify array elements based on conditions.

#### Frequent mistakes & fixes

- **Mistake:** Using `<= data.length`.  
- **Mistake:** Confusing array length (`data.length`) with `String.length()`.  
- **Mistake:** Forgetting arrays are **fixed size**.

#### Example

```java
public static int indexOfMax(int[] arr) {
    int maxIndex = 0;
    for (int i = 1; i < arr.length; i++) {
        if (arr[i] > arr[maxIndex]) {
            maxIndex = i;
        }
    }
    return maxIndex;
}
// Very common FRQ-style helper method.
```

---

### Unit 7 – ArrayList

#### Subtopics & learning goals

- **`ArrayList<E>` declaration and use.**  
- **Methods on the Quick Reference:** `add`, `get`, `set`, `remove`, `size`.  
- **Traversal with index‑based loops.**  
- **Removing elements while traversing.**  [AP Central](https://apcentral.collegeboard.org/courses/ap-computer-science-a/exam)  

#### Key syntax & patterns

```java
ArrayList<String> list = new ArrayList<String>();
list.add("A");
list.add("B");
list.add(1, "X"); // insert at index 1

for (int i = 0; i < list.size(); i++) {
    System.out.println(list.get(i));
}
```

#### Common exam questions

- Implement methods that **filter**, **count**, or **transform** an `ArrayList`.  
- Handle **removal** correctly (usually with index loop and `i--` after `remove`).  

#### Frequent mistakes & fixes

- **Mistake:** Using enhanced for‑loop while removing elements.  
  - **Fix:** Use index loop when you need to remove.  
- **Mistake:** Forgetting `ArrayList` cannot hold primitives (`int` vs. `Integer`).

#### Example

```java
public static void removeShortWords(ArrayList<String> words) {
    for (int i = 0; i < words.size(); i++) {
        if (words.get(i).length() < 3) {
            words.remove(i);
            i--; // adjust index after removal
        }
    }
}
// This pattern appears constantly in ArrayList FRQs.
```

---

### Unit 8 – 2D array

#### Subtopics & learning goals

- **2D array declaration and creation.**  
- **Row-major traversal:** outer loop over rows, inner over columns.  
- **Counting and transforming elements.**  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  

#### Key syntax & patterns

```java
int[][] grid = new int[3][4];

for (int r = 0; r < grid.length; r++) {
    for (int c = 0; c < grid[0].length; c++) {
        grid[r][c] = r + c;
    }
}
```

#### Common exam questions

- Implement methods that **count**, **search**, or **update** cells.  
- Use **helper methods** to compute row/column totals.

#### Frequent mistakes & fixes

- **Mistake:** Using `grid.length` for both rows and columns.  
  - **Fix:** `grid.length` = rows; `grid[0].length` = columns.  
- **Mistake:** Swapping row/column indices.

#### Example

```java
public static int countGreaterThan(int[][] grid, int limit) {
    int count = 0;
    for (int r = 0; r < grid.length; r++) {
        for (int c = 0; c < grid[0].length; c++) {
            if (grid[r][c] > limit) {
                count++;
            }
        }
    }
    return count;
}
// Very similar to typical Q4 FRQ methods.
```

---

### Unit 9 – Inheritance (now enrichment)

> **Current CED:** Inheritance/polymorphism are no longer required exam topics, but some teachers still teach them.  [apcsexamprep.com](https://www.apcsexamprep.com/pages/ap-csa-exam-prep-hub)  

#### Subtopics (enrichment)

- `extends` keyword, superclass vs. subclass.  
- Method overriding, `super` calls.  

#### Example (for understanding, not priority)

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

---

### Unit 10 – Recursion (now enrichment)

> Recursion is de‑emphasized in the new 4‑unit structure; still useful for logic practice.  [apcsexamprep.com](https://www.apcsexamprep.com/pages/ap-csa-exam-prep-hub)  

#### Subtopics (enrichment)

- Base case vs. recursive case.  
- Tracing recursive calls.  

#### Example

```java
public static int sumTo(int n) {
    if (n == 0) {
        return 0;          // base case
    }
    return n + sumTo(n - 1); // recursive case
}
```

---

## 3. Java Quick Reference sheet (explained)

> These are the **only** library methods you can assume on the exam; they’re printed in Bluebook and may be referenced in questions.  [AP Central](https://apcentral.collegeboard.org/courses/ap-computer-science-a/exam)  

### String methods

| Method | Meaning | Example |
|--------|---------|---------|
| `int length()` | Number of characters | `"abc".length()` → `3` |
| `String substring(int beginIndex, int endIndex)` | Substring from `beginIndex` (inclusive) to `endIndex` (exclusive) | `"hello".substring(1, 4)` → `"ell"` |
| `String substring(int beginIndex)` | Substring from `beginIndex` to end | `"hello".substring(2)` → `"llo"` |
| `int indexOf(String str)` | First index of `str`, or `-1` if not found | `"banana".indexOf("na")` → `2` |
| `int compareTo(String other)` | Negative/zero/positive lexicographic comparison | `"apple".compareTo("banana")` < 0 |

> **Pattern:** `substring` is half‑open; `indexOf` returns `-1` when not found; `compareTo` is used for ordering, not equality.

### Math methods

| Method | Meaning | Example |
|--------|---------|---------|
| `int abs(int x)` / `double abs(double x)` | Absolute value | `Math.abs(-5)` → `5` |
| `double pow(double base, double exp)` | `base^exp` | `Math.pow(2, 3)` → `8.0` |
| `double sqrt(double x)` | Square root | `Math.sqrt(25)` → `5.0` |
| `double random()` | Random `0.0 <= x < 1.0` | `(int)(Math.random() * 6) + 1` → 1–6 |

### Integer / Double wrapper methods

| Method | Meaning | Example |
|--------|---------|---------|
| `Integer.parseInt(String s)` | String → `int` | `Integer.parseInt("42")` → `42` |
| `Double.parseDouble(String s)` | String → `double` | `Double.parseDouble("3.14")` → `3.14` |
| `Integer.MIN_VALUE`, `Integer.MAX_VALUE` | Min/max `int` | Use as sentinels |

### ArrayList methods

| Method | Meaning | Example |
|--------|---------|---------|
| `boolean add(E obj)` | Append to end | `list.add("A")` |
| `void add(int index, E obj)` | Insert at index | `list.add(1, "X")` |
| `E get(int index)` | Element at index | `list.get(0)` |
| `E set(int index, E obj)` | Replace element, return old | `list.set(0, "B")` |
| `E remove(int index)` | Remove at index, return removed | `list.remove(2)` |
| `int size()` | Number of elements | `list.size()` |

---

## 4. FRQ deep dive

### The 4 FRQ types and strategies

#### 1. Methods & control structures (Q1)

- **What it tests:** Writing methods with **loops, conditionals, and `String`** operations.  [AP Central](https://apcentral.collegeboard.org/courses/ap-computer-science-a/exam)  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  
- **Strategy:**
  - **Step 1:** Read the **preconditions/postconditions** carefully.  
  - **Step 2:** Identify **inputs**, **outputs**, and **side effects**.  
  - **Step 3:** Sketch pseudocode: loop type, conditions, updates.  
  - **Step 4:** Translate to Java, using Quick Reference methods instead of reinventing.  

#### 2. Class design (Q2)

- **What it tests:** Implementing a class from a **spec table** (fields, constructor, methods).  
- **Strategy:**
  - **Step 1:** Underline each required behavior in the table.  
  - **Step 2:** List fields and their types.  
  - **Step 3:** Write constructor(s) that initialize all fields.  
  - **Step 4:** Implement methods exactly as described; use helper methods if needed.

#### 3. Array/ArrayList data analysis (Q3)

- **What it tests:** Traversal and manipulation of an `ArrayList` (sometimes arrays).  
- **Strategy:**
  - **Step 1:** Decide if you need **index‑based** loop (almost always yes).  
  - **Step 2:** For removal, remember `i--` after `remove`.  
  - **Step 3:** Use standard patterns: sum, count, filter, transform.

#### 4. 2D array (Q4)

- **What it tests:** Row/column traversal, counting, and updating cells.  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  
- **Strategy:**
  - **Step 1:** Write the **double loop skeleton** first.  
  - **Step 2:** Fill in condition and update logic.  
  - **Step 3:** Use helper methods for row/column totals if specified.

### Rubric: what earns points

- **Correct header:** method name, parameters, return type.  
- **Use of required control structures:** loops, `if` statements as specified.  
- **Correct use of arrays/ArrayList/2D arrays:** indices, bounds, `size()` vs. `length`.  
- **Return values and side effects:** correct final state.  
- **Minor syntax errors** (missing semicolon, etc.) usually lose **1 point** at most if intent is clear; logic errors lose more.  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  

### Annotated FRQ‑style examples (paraphrased)

#### Example A – Dog walking (2025 FRQ Q1‑style)  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  

Suppose you must write a method that, given an array of hourly dog counts, returns the **maximum number of dogs** available in any hour.

```java
public int maxDogs(int[] hourlyDogs) {
    int max = hourlyDogs[0];              // +1: correct initialization
    for (int i = 1; i < hourlyDogs.length; i++) { // +1: correct loop bounds
        if (hourlyDogs[i] > max) {        // +1: correct comparison
            max = hourlyDogs[i];          // +1: update
        }
    }
    return max;                           // +1: correct return
}
```

- This would earn full credit for a “max in array” subpart: correct loop, comparison, and return.

#### Example B – 2D grid fill (Q4‑style)

You must count how many cells in a 2D grid contain a value greater than a threshold.

```java
public int countAbove(int[][] grid, int limit) {
    int count = 0;                         // +1: initialization
    for (int r = 0; r < grid.length; r++) {        // +1: row loop
        for (int c = 0; c < grid[0].length; c++) { // +1: column loop
            if (grid[r][c] > limit) {      // +1: condition
                count++;                   // +1: update
            }
        }
    }
    return count;                          // +1: return
}
```

- This matches the pattern of many 2D FRQs: nested loops + conditional count.

---

## 5. MCQ strategy & tricky patterns

### Most commonly tested MCQ concepts

- **Code tracing:** loops, conditionals, method calls.  [Fiveable](https://fiveable.me/ap-comp-sci-a/ap-computer-science-a-exam/ap-comp-sci-a-ap-csa-mcq/study-guide/ap-comp-sci-a-ap-csa-mcq)  
- **Data collections:** arrays, `ArrayList`, 2D arrays.  
- **String and Math methods.**  
- **Class design basics:** fields, constructors, method calls.  

### Tracing under time pressure

- **Step 1:** Identify **what is being asked** (final value, output, count, etc.).  
- **Step 2:** Track only **relevant variables**; ignore noise.  
- **Step 3:** Use a **small table** in your scratch area:

  | Step | i | j | value | output |
  |------|---|---|-------|--------|

- **Step 4:** If stuck, eliminate impossible answers (e.g., wrong type, out‑of‑range).

### Elimination strategies

- **Type mismatch:** If answer type doesn’t match question, eliminate.  
- **Boundary checks:** For loops, check first and last iteration; eliminate answers that violate bounds.  
- **String indices:** If an answer uses invalid indices (e.g., `substring(0, s.length())` is valid; `substring(0, s.length()+1)` is not).

### “Gotcha” patterns

- **Off‑by‑one:** `i <= arr.length` vs. `< arr.length`.  
- **Integer division:** `7 / 2` → `3`, not `3.5`.  
- **`String` equality:** `==` vs. `.equals`.  
- **Null references:** calling methods on `null` (conceptually tested, though they won’t crash Bluebook).  
- **Short‑circuit:** In `a != 0 && b / a > 1`, if `a == 0`, second part is never evaluated.

---

## 6. Algorithms & logic patterns to master

### Searches

- **Sequential (linear) search:**

  ```java
  public static int linearSearch(int[] arr, int target) {
      for (int i = 0; i < arr.length; i++) {
          if (arr[i] == target) {
              return i;
          }
      }
      return -1;
  }
  ```

- **Binary search** (on **sorted** arrays):

  ```java
  public static int binarySearch(int[] arr, int target) {
      int low = 0;
      int high = arr.length - 1;
      while (low <= high) {
          int mid = (low + high) / 2;
          if (arr[mid] == target) return mid;
          else if (arr[mid] < target) low = mid + 1;
          else high = mid - 1;
      }
      return -1;
  }
  ```

### Sorting

- **Selection sort:**

  ```java
  public static void selectionSort(int[] arr) {
      for (int i = 0; i < arr.length - 1; i++) {
          int minIndex = i;
          for (int j = i + 1; j < arr.length; j++) {
              if (arr[j] < arr[minIndex]) {
                  minIndex = j;
              }
          }
          int temp = arr[i];
          arr[i] = arr[minIndex];
          arr[minIndex] = temp;
      }
  }
  ```

- **Insertion sort:**

  ```java
  public static void insertionSort(int[] arr) {
      for (int i = 1; i < arr.length; i++) {
          int key = arr[i];
          int j = i - 1;
          while (j >= 0 && arr[j] > key) {
              arr[j + 1] = arr[j];
              j--;
          }
          arr[j + 1] = key;
      }
  }
  ```

### Recursion tracing (enrichment)

- Write out **call stack**:

  ```java
  f(3)
    -> 3 + f(2)
           -> 2 + f(1)
                  -> 1 + f(0)
                         -> 0
  ```

### String traversal patterns

- **Count characters with a property.**  
- **Build a new string** by concatenation.  

```java
public static String removeSpaces(String s) {
    String result = "";
    for (int i = 0; i < s.length(); i++) {
        char c = s.charAt(i);
        if (c != ' ') {
            result += c;
        }
    }
    return result;
}
```

### Array/ArrayList manipulation patterns

- **Filter:** keep/remove elements based on condition.  
- **Transform:** modify each element (e.g., multiply by 2).  
- **Aggregate:** sum, average, min, max.

---

## 7. Priority study matrix

> Rough weights based on current emphasis: data collections + control structures dominate.  [Fiveable](https://fiveable.me/ap-comp-sci-a/ap-computer-science-a-exam/ap-comp-sci-a-ap-csa-mcq/study-guide/ap-comp-sci-a-ap-csa-mcq)  [apcsexamprep.com](https://www.apcsexamprep.com/pages/ap-csa-exam-prep-hub)  

| Topic | Exam Weight | Difficulty | Priority Level | Time to Allocate (hrs) |
|-------|-------------|------------|----------------|------------------------|
| Loops & conditionals (Units 3–4) | Very High | Medium | **Top** | 15–20 |
| Arrays (Unit 6) | High | Medium | **Top** | 12–15 |
| ArrayList (Unit 7) | High | Medium | **Top** | 12–15 |
| 2D arrays (Unit 8) | High | Medium–High | **Top** | 10–12 |
| Class design (Unit 5) | Medium | Medium–High | High | 10–12 |
| Strings & Math APIs (Unit 2) | Medium | Medium | High | 8–10 |
| Primitive types & expressions (Unit 1) | Medium | Low–Medium | High | 6–8 |
| Searching & sorting algorithms | Medium | Medium–High | High | 8–10 |
| Recursion (enrichment) | Low | High | Low | 3–4 |
| Inheritance (enrichment) | ~0 | Medium | Lowest | 0–2 |

---

## 8. Complete 8‑week study plan

Assume ~**1.5–2 hours/day, 6 days/week** (≈ 12 hours/week). Adjust up/down as needed.

### Week 1 – Foundations

- **Topics:** Units 1–2 (primitive types, expressions, using objects, `String`, `Math`).  
- **Daily (≈2h):**
  - **1h:** Read notes / watch short videos (Khan Academy, CS Awesome).  [AP Students | College Board](https://apstudents.collegeboard.org/courses/ap-computer-science-a)  [Reddit](https://www.reddit.com/r/APStudents/comments/rfmmf5/self_studying_for_ap_computer_science_a_apcsa/)  
  - **1h:** CodingBat warmups (`Warmup-1`, `String-1`).  [codingbat.com](https://codingbat.com/java)  
- **Milestone:** Comfortably evaluate expressions and use `String`/`Math` methods.

### Week 2 – Conditionals & basic loops

- **Topics:** Unit 3 + intro Unit 4.  
- **Daily:**
  - **45 min:** Practice `if`/`if-else` and Boolean logic.  
  - **45 min:** Simple `while`/`for` loops.  
  - **30 min:** 10–15 MCQs from AP‑style sources (AP Classroom, CS Awesome, Fiveable).  [Fiveable](https://fiveable.me/ap-comp-sci-a/ap-computer-science-a-exam/ap-comp-sci-a-ap-csa-mcq/study-guide/ap-comp-sci-a-ap-csa-mcq)  [AP Students | College Board](https://apstudents.collegeboard.org/courses/ap-computer-science-a)  
- **Milestone:** Trace and write simple loops and conditionals without hesitation.

### Week 3 – Loop mastery & String traversal

- **Topics:** Deeper Unit 4; String traversal.  
- **Daily:**
  - **1h:** CodingBat `String-2`, `Logic-1`, loop problems.  [codingbat.com](https://codingbat.com/java)  [codingbat.com](https://codingbat.com/java/AP-1)  
  - **1h:** Timed MCQ sets (10–15 questions).  
- **Milestone:** Confident with nested loops and counting patterns.

### Week 4 – Arrays

- **Topics:** Unit 6 + search/sort basics.  
- **Daily:**
  - **1h:** Implement linear search, selection sort, insertion sort.  
  - **1h:** AP Classroom / released MCQs on arrays + 1 array FRQ subpart.  [skylit.com](https://skylit.com/beprepared/2025-CED-Sample-MC-Solutions.pdf)  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  
- **Milestone:** Can write array traversal methods from scratch.

> **By end of Week 4:** Finish solid coverage of Units 1–6 and most MCQ practice for them.

### Week 5 – ArrayList & FRQ practice

- **Topics:** Unit 7 + FRQ Q3 style.  
- **Daily:**
  - **45 min:** ArrayList coding drills (add, remove, filter).  
  - **45 min:** One FRQ Q3‑style question (past exam or CED sample).  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  [apcsexamprep.com](https://www.apcsexamprep.com/pages/ap-csa-exam-prep-hub)  
  - **30 min:** Review Java Quick Reference methods.  [AP Central](https://apcentral.collegeboard.org/courses/ap-computer-science-a/exam)  
- **Milestone:** Comfortable with ArrayList traversal and removal patterns.

### Week 6 – 2D arrays & full FRQs

- **Topics:** Unit 8 + FRQ Q4 style.  
- **Daily:**
  - **1h:** 2D array coding (row/column sums, counts, transforms).  
  - **1h:** Alternate between Q1 and Q4 FRQs from past exams.  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  [altareen.github.io](https://altareen.github.io/csa/frqs/)  
- **Milestone:** Can write nested loops for 2D arrays quickly and correctly.

### Week 7 – Class design & mixed practice

- **Topics:** Unit 5 + full exam simulation.  
- **Daily:**
  - **45 min:** Class design FRQs (Q2).  
  - **45 min:** Mixed MCQ sets (arrays, ArrayList, 2D, loops).  
  - **30 min:** Review mistakes and update a personal “error log”.
- **Milestone:** Complete at least **4 full FRQs** under time (≈20–22 min each).

### Week 8 – Review & exam simulation

- **Topics:** All high‑priority topics; light recursion/inheritance if desired.  
- **Daily:**
  - **Day 1–3:** Take **one full practice exam** (42 MCQ + 4 FRQ) every other day (Barron’s, Princeton, AP Classroom).  [Target](https://www.target.com/p/ap-computer-science-a-premium-13th-edition-prep-book-with-6-practice-tests-comprehensive-review-online-practice-barron-s-ap-prep/-/A-1006898838)  [Google Books](https://books.google.com/books/about/Princeton_Review_AP_Computer_Science_A_P.html?id=Kdq0EAAAQBAJ)  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  
  - **Day 4–6:** Targeted review of weakest areas from those exams.  
- **Milestone:** Finish at least **2 full timed exams** with score trending toward 4–5.

---

## 9. Best free & paid resources

### Free online resources

- **AP Classroom (College Board):** Official MCQs, progress checks, and FRQs aligned to the new CED.  [AP Students | College Board](https://apstudents.collegeboard.org/courses/ap-computer-science-a)  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap25-frq-computer-science-a.pdf)  
- **CS Awesome (Runestone):** Free interactive textbook with AP CSA‑aligned units, code examples, and practice.  [Reddit](https://www.reddit.com/r/APStudents/comments/rfmmf5/self_studying_for_ap_computer_science_a_apcsa/)  
- **CodingBat (Java):** Short, focused problems—especially good for loops, strings, arrays, and AP‑style logic.  [codingbat.com](https://codingbat.com/java)  [codingbat.com](https://codingbat.com/java/AP-1)  
- **GitHub FRQ repos:**  
  - FRQ archives and solutions with explanations.  [altareen.github.io](https://altareen.github.io/csa/frqs/)  [Github](https://github.com/Codeboid/ap-cs-frq-series)  

### YouTube channels (search terms)

- **“AP CSA 2025 CS Awesome”**, **“AP CSA FRQ walkthrough 2025/2024”**—look for channels that explicitly reference the **new 4‑unit curriculum** and 42‑MCQ format.  [skylit.com](https://skylit.com/beprepared/2025-CED-Sample-MC-Solutions.pdf)  [apcsexamprep.com](https://www.apcsexamprep.com/pages/ap-csa-exam-prep-hub)  

### CodeHS / Codecademy / Khan Academy

- **CodeHS AP CSA course:** Structured Java curriculum with autograded problems; good if your school provides access.  [Reddit](https://www.reddit.com/r/APStudents/comments/rfmmf5/self_studying_for_ap_computer_science_a_apcsa/)  
- **Khan Academy programming:** Great for foundational logic and practice, though not AP‑specific.  [AP Students | College Board](https://apstudents.collegeboard.org/courses/ap-computer-science-a)  

### Prep books (paid)

| Book | Strengths | Notes |
|------|-----------|-------|
| **Barron’s AP Computer Science A Premium (13th ed., 2026)** | Very thorough content review, 6 practice tests, updated for 2025–26 CED.  [Target](https://www.target.com/p/ap-computer-science-a-premium-13th-edition-prep-book-with-6-practice-tests-comprehensive-review-online-practice-barron-s-ap-prep/-/A-1006898838) | Great if you want depth and many practice questions. |
| **Princeton Review AP CSA Premium (9th ed., for new 2026 exam)** | Strong strategies, 5 practice tests, concise review.  [Google Books](https://books.google.com/books/about/Princeton_Review_AP_Computer_Science_A_P.html?id=Kdq0EAAAQBAJ)  [Amazon Singapore](https://www.amazon.sg/Princeton-Review-Computer-Science-Prep/dp/0593517059) | Good if you like exam‑strategy focus. |

### Anki decks

- **APCS – Java Concepts deck (AnkiWeb):** Vocabulary and concept cards aligned with a Java AP textbook.  [AnkiWeb](https://ankiweb.net/shared/info/1951790685)  
- You can also build your own deck from **your error log** and Quick Reference methods.

### Communities

- **r/APStudents** and **r/AP_CompSci** on Reddit: exam discussions, resource links, and study tips.  [Reddit](https://www.reddit.com/r/APStudents/comments/rfmmf5/self_studying_for_ap_computer_science_a_apcsa/)  [Reddit](https://www.reddit.com/r/APStudents/comments/g2hcv8/computer_science_a_vs_principles/)  
- **AP Students Discord server:** Large community with subject channels, including AP CSA.  [Discord](https://discord.com/invite/apstudents)  [Discord Bot List](https://discordbotlist.com/servers/apstudents)  

---

## 10. Exam day strategy

### Time management

- **MCQ (42 Q / 90 min):**
  - Aim for **~2 min per question**.  
  - First pass: answer all **easy/medium** questions; mark hard ones.  
  - Second pass: spend remaining time on marked questions.

- **FRQ (4 Q / 90 min):**
  - Plan **~20 min per question**, with **10 min buffer**.  
  - Suggested order: Q2 (Class) → Q1 (Methods) → Q3 (ArrayList) → Q4 (2D), or your personal strength order.

### When you’re stuck on a coding question

- **MCQ:**  
  - Eliminate obviously wrong answers (type errors, out‑of‑range values).  
  - If still unsure, **guess**—there’s no penalty.

- **FRQ:**  
  - Write **partial solutions**: correct header, loop skeleton, and comments describing intended logic.  
  - Use **helper methods** if a subtask is hard; implement the easier parts fully.

### Writing for partial credit (FRQ)

- Always include:
  - **Correct method header** (name, parameters, return type).  
  - **Reasonable control structure** (even if condition is slightly off).  
  - **Return statement** of the right type.  
- If you can’t finish logic, **comment your intent** (e.g., `// find max in array here`). The grader can see your thinking.

### Mental checklist before submitting each FRQ

- **Header:** Is the method/class signature exactly as specified?  
- **Parameters:** Are types and names correct?  
- **Return:** Does every path return a value of the correct type?  
- **Loops:** Are bounds correct (`< length`, `< size()`, correct row/column lengths)?  
- **APIs:** Are `substring`, `indexOf`, `size`, `length`, `add`, `remove` used with correct parameters?  
- **Side effects:** Did you update the right field/array/ArrayList?

---

If you want, next step we can turn this into **printable checklists** or **unit‑specific practice sets** (e.g., “Unit 4 loop patterns only”) so you can plug them straight into your study routine or club materials.
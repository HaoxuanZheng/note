# AP Precalculus Master Study Guide (2025–2026)

You’re aiming for a 5—so this will be **exam‑aligned, brutally focused, and strategy‑driven**, not just a topic dump.

---

## 1. Full exam overview

### 1.1 Exam format

**Total time:** 3 hours  
**Sections:**  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus/exam)  [AP Students | College Board](https://apstudents.collegeboard.org/courses/ap-precalculus/assessment)  

- **Section I: Multiple Choice — 40 questions, 2 hours, 62.5%**
  - **Part A:** 28 questions, 80 minutes, **no calculator**, ~43.75%
  - **Part B:** 12 questions, 40 minutes, **graphing calculator required (Desmos in Bluebook)**, ~18.75%
- **Section II: Free Response — 4 questions, 1 hour, 37.5%**
  - **Part A:** 2 questions, 30 minutes, **calculator required**
    - Q1: Function concepts  
    - Q2: Modeling a non‑periodic context
  - **Part B:** 2 questions, 30 minutes, **no calculator**
    - Q3: Modeling a periodic context  
    - Q4: Symbolic manipulations  

Units tested (MCQ weighting):  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus)  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus)  

- **Unit 1: Polynomial & Rational** — 30–40%  
- **Unit 2: Exponential & Logarithmic** — 27–40%  
- **Unit 3: Trigonometric & Polar** — 30–35%  
- **Unit 4: Parameters, Vectors, Matrices** — **not on the exam**, but excellent prep for later math.

### 1.2 Calculator policy (Desmos)

- **Calculator allowed:**
  - Section I Part B (12 MCQ)
  - Section II Part A (2 FRQ)
- **Calculator not allowed:**
  - Section I Part A (28 MCQ)
  - Section II Part B (2 FRQ)
- The exam uses **built‑in Desmos in Bluebook**, not the web/app version.  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus/exam/graphing-calculators)  

**Key idea:** Most of the exam is **non‑calculator**—you must be fluent symbolically.

### 1.3 Composite score → AP 1–5

College Board does **not** publish an exact conversion. Each year, raw scores (MCQ + FRQ) are scaled to 1–5. Roughly:

- **MCQ:** 40 questions, 62.5% of score  
- **FRQ:** 4 questions × 6 points = 24 raw FRQ points, 37.5%  

Heuristically (not official):

- **5:** high 70s–80%+ of total scaled points  
- **4:** ~60–75%  
- **3:** ~45–60%  

Treat this as **guidance**, not a guarantee.

### 1.4 AP Precalculus vs “regular” Precalculus

**AP Precalculus:**

- Built around **modeling and functions** with multiple representations (symbolic, numeric, graphical, verbal).  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus)  [AP Students | College Board](https://apstudents.collegeboard.org/courses/ap-precalculus)  
- Heavy emphasis on:
  - Interpreting graphs and tables
  - Justifying reasoning in words
  - Real‑world modeling (non‑periodic and periodic)
- Unit 4 (vectors/matrices/parameters) is **course content**, but **not tested** on the AP exam.

**Typical school Precalculus:**

- Often broader but less standardized: conics, sequences/series, limits, more trig identities, etc.
- Less emphasis on **written justification** and **AP‑style modeling FRQs**.

---

## 2. Unit‑by‑unit content breakdown

I’ll align with the CED structure (all learning objectives are essentially combinations of: interpret, represent, build, transform, and solve with functions).  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap-precalculus-course-and-exam-description.pdf)  [AP Central](https://apcentral.collegeboard.org/media/pdf/ap-precalculus-course-and-exam-description.pdf)  

For each unit:

- **Concept overview**
- **2 worked examples (medium + hard)**
- **Common exam formats**
- **Classic misconceptions**

---

### Unit 1 – Polynomial and Rational Functions

#### 2.1 Core learning goals (clustered)

- **Rates of change & modeling with polynomials**
- **Structure of polynomials: degree, leading term, zeros, multiplicity**
- **End behavior and local/global behavior**
- **Rational functions: asymptotes, holes, domain, intercepts**
- **Polynomial division, Remainder Theorem, equivalent forms**
- **Inequalities with polynomial/rational expressions**
- **Choosing and justifying function models**

#### 2.2 Key concepts & explanations

**Power functions & end behavior**

- A **power function**: \(f(x) = kx^n\) with real \(k\), integer \(n\).
- **End behavior** driven by:
  - Sign of \(k\)
  - Parity of \(n\) (even/odd)
- Example:
  - \(f(x) = -2x^3\): as \(x \to \infty\), \(f(x) \to -\infty\); as \(x \to -\infty\), \(f(x) \to \infty\).

**Polynomials: zeros & multiplicity**

- If \(f(x) = a(x-r_1)^{m_1}(x-r_2)^{m_2}\cdots\), then:
  - Zeros at \(x = r_i\)
  - **Multiplicity** \(m_i\):
    - Odd multiplicity → graph **crosses** the x‑axis.
    - Even multiplicity → graph **touches/bounces**.

**Rational functions**

- \(f(x) = \dfrac{p(x)}{q(x)}\), \(q(x)\neq 0\).
- **Vertical asymptotes:** where \(q(x)=0\) and factor **does not cancel**.
- **Holes:** common factor cancels between numerator and denominator.
- **Horizontal/slant asymptotes:** compare degrees of \(p\) and \(q\).

**Polynomial division & Remainder Theorem**

- Divide \(p(x)\) by \((x-a)\):  
  \(p(x) = (x-a)q(x) + r\), where \(r = p(a)\).
- If \(p(a)=0\), then \((x-a)\) is a factor.

**Inequalities**

- Solve \( \dfrac{p(x)}{q(x)} > 0\) by:
  - Finding zeros of numerator and denominator.
  - Creating a sign chart on intervals.

#### 2.3 Worked examples

##### Example 1 (medium) – End behavior & multiplicity

**Problem:**  
\(f(x) = -2(x+1)^2(x-3)^3\)

1. **End behavior**
   - Degree: \(2+3=5\) (odd), leading coefficient \(-2\) (negative).
   - As \(x \to \infty\), \(f(x) \to -\infty\); as \(x \to -\infty\), \(f(x) \to \infty\).

2. **Behavior at zeros**
   - Zero at \(-1\), multiplicity 2 → touches/bounces.
   - Zero at \(3\), multiplicity 3 → crosses with flattening.

**Exam‑style question:** “Which graph could represent \(f\)?” You match:

- Right tail down, left tail up.
- Bounce at \(-1\), cross at \(3\).

##### Example 2 (hard) – Rational function analysis

**Problem:**  
\(f(x) = \dfrac{(x-1)(x+2)}{(x-1)(x-4)}\)

1. **Simplify (for analysis only):**  
   \(f(x) = \dfrac{x+2}{x-4}\), but **note** \(x\neq 1\) (hole).

2. **Domain:** all real \(x\) except \(x=1,4\).

3. **Vertical asymptote:** \(x=4\) (denominator zero, no cancellation).

4. **Hole:** at \(x=1\).  
   - y‑value: plug into simplified form: \(\dfrac{1+2}{1-4} = \dfrac{3}{-3} = -1\).  
   - Hole at \((1,-1)\).

5. **Horizontal asymptote:** degrees equal → \(y = \dfrac{1}{1} = 1\).

**Typical FRQ twist:** interpret a context (e.g., rate, concentration) and explain what the hole/asymptote means physically.

#### 2.4 Common exam formats

- MCQ: “Which graph matches this factored polynomial?”  
- MCQ: “Which statement about end behavior is true?”  
- FRQ: modeling with a polynomial or rational function, interpreting zeros/asymptotes, justifying model choice.

#### 2.5 Misconceptions

- **Thinking holes are asymptotes** (they’re not; they’re removable discontinuities).
- Forgetting to **exclude canceled factors** from the domain.
- Misreading multiplicity (assuming every zero crosses).
- Treating end behavior as local behavior near the origin.

---

### Unit 2 – Exponential and Logarithmic Functions

#### 2.6 Core learning goals

- **Arithmetic vs geometric sequences; linear vs exponential growth**
- **Exponential functions & parameters (initial value, growth/decay factor)**
- **Properties of exponents and logs**
- **Natural log and base \(e\)**
- **Solving exponential/log equations and inequalities**
- **Modeling data with exponentials/logs; semi‑log plots**  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus)  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus)  

#### 2.7 Key concepts

**Exponential models**

- General form: \(f(t) = a\cdot b^t\) or \(f(t) = ae^{kt}\).
  - \(a\): initial value.
  - \(b>1\) or \(k>0\): growth; \(0<b<1\) or \(k<0\): decay.

**Logarithms**

- \(\log_b(x)\) is the inverse of \(b^x\).
- Key identities:
  - \(\log_b(xy) = \log_b x + \log_b y\)
  - \(\log_b\left(\dfrac{x}{y}\right) = \log_b x - \log_b y\)
  - \(\log_b(x^k) = k\log_b x\)
  - Change of base: \(\log_b x = \dfrac{\ln x}{\ln b}\)

**Semi‑log plots**

- Plot \((x, \log y)\) to linearize an exponential:  
  If \(y = ab^x\), then \(\log y = \log a + x\log b\) (a line).

#### 2.8 Worked examples

##### Example 1 (medium) – Exponential equation

**Problem:**  
Solve \(500\cdot 1.08^t = 800\) for \(t\).

1. Divide: \(1.08^t = \dfrac{800}{500} = 1.6\).
2. Take logs:  
   \(t\ln(1.08) = \ln(1.6)\).
3. \(t = \dfrac{\ln(1.6)}{\ln(1.08)} \approx 5.9\).

**Exam angle:** interpret “after how many years does the investment reach \$800?”

##### Example 2 (hard) – Semi‑log linearization

**Problem:**  
Data for a population \(P(t)\) is given. A semi‑log plot of \((t,\ln P)\) is approximately linear with slope \(0.12\) and intercept \(4.5\). Find a model.

1. Line: \(\ln P = 0.12t + 4.5\).
2. Exponentiate:  
   \(P = e^{0.12t + 4.5} = e^{4.5}\cdot e^{0.12t}\).
3. So \(P(t) \approx Ae^{0.12t}\) with \(A = e^{4.5}\).

**Typical FRQ:** ask you to interpret slope (growth rate) and intercept (initial value) in context.

#### 2.9 Common formats & misconceptions

**Formats**

- MCQ: solving exponential/log equations, interpreting graphs, comparing growth rates.
- FRQ: modeling with exponentials, interpreting parameters, using semi‑log plots.

**Misconceptions**

- Treating \(\log(x+y)\) as \(\log x + \log y\) (false).
- Forgetting domain restrictions: \(\log(x)\) requires \(x>0\).
- Confusing **growth factor** \(b\) with **growth rate** (e.g., 8% growth → \(b=1.08\), rate \(0.08\)).

---

### Unit 3 – Trigonometric and Polar Functions

#### 2.10 Core learning goals

- **Periodic phenomena and sinusoidal modeling**
- **Unit circle values (degrees & radians)**
- **Graphs of sine, cosine, tangent and transformations**
- **Amplitude, period, phase shift, vertical shift**
- **Inverse trig functions, domains/ranges**
- **Trig identities and solving trig equations**
- **Polar coordinates and polar graphs**  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus)  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus)  

#### 2.11 Unit circle essentials

**Key angles (degrees / radians) and \((\cos\theta,\sin\theta)\):**

- \(0^\circ\) / \(0\): \((1,0)\)
- \(30^\circ\) / \(\pi/6\): \(\left(\dfrac{\sqrt{3}}{2},\dfrac{1}{2}\right)\)
- \(45^\circ\) / \(\pi/4\): \(\left(\dfrac{\sqrt{2}}{2},\dfrac{\sqrt{2}}{2}\right)\)
- \(60^\circ\) / \(\pi/3\): \(\left(\dfrac{1}{2},\dfrac{\sqrt{3}}{2}\right)\)
- \(90^\circ\) / \(\pi/2\): \((0,1)\)
- And symmetric points in quadrants II–IV with sign changes.

**Six trig functions**

- \(\sin\theta = \dfrac{\text{opposite}}{\text{hypotenuse}}\), \(\cos\theta = \dfrac{\text{adjacent}}{\text{hypotenuse}}\), \(\tan\theta = \dfrac{\sin\theta}{\cos\theta}\).
- \(\csc\theta = 1/\sin\theta\), \(\sec\theta = 1/\cos\theta\), \(\cot\theta = 1/\tan\theta\).

**Transformations**

- \(y = A\sin(B(x-C)) + D\)
  - **Amplitude:** \(|A|\)
  - **Period:** \(\dfrac{2\pi}{|B|}\)
  - **Phase shift:** \(C\)
  - **Vertical shift:** \(D\)

**Inverse trig**

- \(\sin^{-1}x\) (arcsin): domain \([-1,1]\), range \([-\pi/2,\pi/2]\).
- \(\cos^{-1}x\): domain \([-1,1]\), range \([0,\pi]\).
- \(\tan^{-1}x\): domain \(\mathbb{R}\), range \((-\pi/2,\pi/2)\).

**Polar coordinates**

- Point: \((r,\theta)\) with \(r\ge 0\).
- Conversion:
  - \(x = r\cos\theta\), \(y = r\sin\theta\).
  - \(r = \sqrt{x^2 + y^2}\), \(\theta = \tan^{-1}\left(\dfrac{y}{x}\right)\) (adjust quadrant).

#### 2.12 Worked examples

##### Example 1 (medium) – Sinusoidal model

**Problem:**  
A temperature varies between \(10^\circ\) and \(30^\circ\) with a period of 24 hours. Max at \(t=6\) hours. Find a model \(T(t)\).

1. **Midline:** \(\dfrac{10+30}{2} = 20\).  
2. **Amplitude:** \(\dfrac{30-10}{2} = 10\).  
3. **Period:** 24 → \(B = \dfrac{2\pi}{24} = \dfrac{\pi}{12}\).  
4. Max at \(t=6\) → use cosine shifted:  
   \(T(t) = 20 + 10\cos\left(\dfrac{\pi}{12}(t-6)\right)\).

**Exam twist:** interpret \(B\) as “how quickly the cycle repeats,” or ask for time when \(T=25\).

##### Example 2 (hard) – Polar to rectangular & graph behavior

**Problem:**  
\(r = 2\cos\theta\).

1. Convert to rectangular:
   - \(r = \sqrt{x^2 + y^2}\), \(x = r\cos\theta\).
   - \(r = 2\cos\theta \Rightarrow r = 2\cdot \dfrac{x}{r} \Rightarrow r^2 = 2x\).
   - So \(x^2 + y^2 = 2x\) → \(x^2 - 2x + y^2 = 0\) → \((x-1)^2 + y^2 = 1\).
   - Circle of radius 1 centered at \((1,0)\).

2. Graph: circle to the right of origin.

**Typical MCQ:** “Which graph matches \(r = 2\cos\theta\)?” or “Which equation in rectangular form is equivalent?”

#### 2.13 Common formats & misconceptions

**Formats**

- MCQ: identify amplitude/period/phase shift from equation or graph.
- MCQ: convert between polar and rectangular, identify polar graphs (rose, circle, limaçon).
- FRQ: periodic modeling (Q3), interpret parameters, solve for times.

**Misconceptions**

- Mixing degrees and radians (AP expects **radians** in calculator sections).  [AP Students | College Board](https://apstudents.collegeboard.org/courses/ap-precalculus/assessment)  
- Misidentifying amplitude vs vertical shift.
- Forgetting that polar points can represent the same location with different \((r,\theta)\).

---

### Unit 4 – Functions with Parameters, Vectors, Matrices  
*(Not on the exam, but powerful for understanding.)*

#### 2.14 Core learning goals

- **Parametric equations and eliminating parameters**
- **Vectors: magnitude, direction, components, operations**
- **Dot product and angle between vectors**
- **Matrices: addition, scalar multiplication, multiplication**
- **Matrix inverses and solving systems**
- **Linear transformations via matrices**  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus)  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus)  

#### 2.15 Key concepts & quick examples

**Parametric**

- Example: projectile motion  
  \(x(t) = v_0\cos\theta\cdot t\), \(y(t) = v_0\sin\theta\cdot t - \dfrac{1}{2}gt^2\).
- Eliminate \(t\) to get a relation between \(x\) and \(y\).

**Vectors**

- \(\vec{v} = \langle a,b\rangle\), magnitude \(|\vec{v}| = \sqrt{a^2 + b^2}\).
- Dot product: \(\vec{u}\cdot\vec{v} = u_1v_1 + u_2v_2 = |\vec{u}||\vec{v}|\cos\theta\).

**Matrices**

- Multiply \(A_{m\times n}B_{n\times p}\) to get \(C_{m\times p}\).
- Solve \(A\vec{x} = \vec{b}\) via \(A^{-1}\vec{b}\) when \(A\) is invertible.

*(Since Unit 4 is not tested, we’ll keep it as enrichment.)*

---

## 3. Formula master sheet

**Legend:**  
- **GIVEN** = appears on AP formula sheet or is effectively provided by context.  
- **MEMORIZE** = you must know it cold.

### 3.1 Unit 1 – Polynomial & Rational

- **End behavior:** determined by leading term \(a_nx^n\). (**Concept**, not formula)
- **Remainder Theorem:** \(p(a)\) is remainder when dividing by \((x-a)\). (**MEMORIZE**)
- **Factor Theorem:** \(p(a)=0 \Leftrightarrow (x-a)\) is a factor. (**MEMORIZE**)

### 3.2 Unit 2 – Exponential & Log

- **Exponential forms:**
  - \(y = ab^x\), \(y = ae^{kx}\). (**MEMORIZE**)
- **Log rules (all MEMORIZE):**
  - \(\log_b(xy) = \log_b x + \log_b y\)
  - \(\log_b\left(\dfrac{x}{y}\right) = \log_b x - \log_b y\)
  - \(\log_b(x^k) = k\log_b x\)
  - \(\log_b x = \dfrac{\ln x}{\ln b}\)

### 3.3 Unit 3 – Trig & Polar

**Pythagorean identities (MEMORIZE):**

- \(\sin^2\theta + \cos^2\theta = 1\)
- \(1 + \tan^2\theta = \sec^2\theta\)
- \(1 + \cot^2\theta = \csc^2\theta\)

**Even/odd (MEMORIZE):**

- \(\sin(-\theta) = -\sin\theta\), \(\cos(-\theta) = \cos\theta\), \(\tan(-\theta) = -\tan\theta\).

**Co‑function (MEMORIZE):**

- \(\sin\theta = \cos\left(\dfrac{\pi}{2}-\theta\right)\), etc.

**Angle addition (nice to know, sometimes GIVEN in context):**

- \(\sin(\alpha\pm\beta) = \sin\alpha\cos\beta \pm \cos\alpha\sin\beta\)
- \(\cos(\alpha\pm\beta) = \cos\alpha\cos\beta \mp \sin\alpha\sin\beta\)

**Polar conversion (MEMORIZE):**

- \(x = r\cos\theta\), \(y = r\sin\theta\)
- \(r = \sqrt{x^2 + y^2}\), \(\theta = \tan^{-1}\left(\dfrac{y}{x}\right)\) (quadrant‑aware)

**Law of Sines & Cosines** (not central but useful):

- Law of Sines: \(\dfrac{a}{\sin A} = \dfrac{b}{\sin B} = \dfrac{c}{\sin C}\)
- Law of Cosines: \(c^2 = a^2 + b^2 - 2ab\cos C\)

### 3.4 Unit 4 – Vectors & Matrices

- \(|\vec{v}| = \sqrt{v_1^2 + v_2^2}\)
- \(\vec{u}\cdot\vec{v} = u_1v_1 + u_2v_2 = |\vec{u}||\vec{v}|\cos\theta\)
- Matrix multiplication rules (conceptual, not formula).

---

## 4. Desmos calculator mastery

Based on College Board’s expectations for graphing calculators in AP Precalculus.  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus/exam/graphing-calculators)  [Desmos](https://www.desmos.com/calculator)  

### 4.1 What Desmos must do for you

- Graph functions and analyze:
  - Intersections, zeros, minima/maxima
- Generate tables
- Find numerical solutions to equations
- Perform regressions (linear, quadratic, cubic, quartic, exponential, logarithmic, sinusoidal)
- Plot residuals

### 4.2 Top 10 Desmos tricks (exam‑relevant)

1. **Graph quickly:** type `y =` or `f(x) =` and enter expressions; use sliders for parameters.
2. **Find zeros:** click on x‑axis intercepts; Desmos shows coordinates.
3. **Intersections:** graph two functions, tap intersection point.
4. **Min/max:** tap local extrema points.
5. **Tables:** type `f(x)=...`, then add table; Desmos auto‑fills \(f(x)\).
6. **Regression:** enter data in a table, then type `y1 ~ a x1 + b` (or other model) to fit.
7. **Sinusoidal regression:** `y1 ~ a sin(bx1 + c) + d`.
8. **Zoom smart:** use zoom fit to see all relevant behavior.
9. **Check periodicity:** graph several cycles to confirm period and amplitude.
10. **Compare models:** overlay multiple candidate functions and visually inspect fit.

### 4.3 When to use Desmos vs by hand

**Use Desmos when:**

- The question explicitly says “calculator permitted/required.”
- You need:
  - Regression
  - Numerical solutions that are messy
  - Quick graph behavior (e.g., number of intersections)

**Work by hand when:**

- Section I Part A or Section II Part B.
- Algebraic manipulation is straightforward (solving simple exponentials/logs, factoring polynomials).

### 4.4 Desmos‑targeted practice prompts

- **Prompt 1:** Given a data table, use Desmos to fit an exponential model and interpret parameters.
- **Prompt 2:** Graph a rational function, identify asymptotes, zeros, and holes; then justify algebraically.
- **Prompt 3:** Use sinusoidal regression to model periodic data and predict future values.

---

## 5. FRQ strategy & sample responses

### 5.1 FRQ structure

- **4 questions, 6 points each**:
  - Q1: Function concepts (often multi‑representation)
  - Q2: Non‑periodic modeling (often exponential/polynomial)
  - Q3: Periodic modeling (trig)
  - Q4: Symbolic manipulations (often algebraic/trig/log)

Each question typically has **subparts (a)–(d)**, each worth 1–2 points.

### 5.2 Scoring rubric essentials

You earn points for:

- **Correct setup** (equations, expressions, inequalities)
- **Correct reasoning** (explaining why, not just what)
- **Correct answer** (numeric or algebraic)
- **Communication** (units, context, clear statements)

Calculator use is fine, but you must:

- Indicate **what** you computed (e.g., “Solve \(f(t)=20\) using graph intersection”).
- Provide **rounded answers with units** when appropriate.

### 5.3 Sample FRQ (sketch)

#### Sample FRQ 1 – Non‑periodic modeling (calculator)

**Prompt (condensed):**  
A population \(P(t)\) (in thousands) is modeled by \(P(t) = 12e^{0.04t}\), where \(t\) is years since 2020.

1. (a) Interpret \(P(0)\) and \(0.04\) in context.  
2. (b) Find the average rate of change of \(P\) on \([0,5]\).  
3. (c) Use Desmos to find when \(P(t)=20\).  
4. (d) A second model \(Q(t)\) is linear and fits the same data at \(t=0\) and \(t=5\). Which model better represents long‑term behavior? Justify.

**Annotated solution (sketch):**

- (a)  
  - \(P(0)=12\): initial population is 12 thousand in 2020.  
  - \(0.04\): continuous growth rate of 4% per year.

- (b)  
  \[
  \text{Avg rate} = \frac{P(5)-P(0)}{5} = \frac{12e^{0.2}-12}{5}\ \text{thousand per year}.
  \]

- (c)  
  - In Desmos, graph \(y=12e^{0.04t}\) and \(y=20\), find intersection \(t\approx 13.1\).  
  - State: “The population reaches 20 thousand about 13.1 years after 2020, i.e., in 2033.”

- (d)  
  - Exponential model grows faster than linear for large \(t\).  
  - Justify: “Because the context suggests percentage growth, the exponential model better represents long‑term behavior.”

#### Sample FRQ 2 – Periodic modeling (no calculator)

**Prompt (condensed):**  
A function \(H(t) = 3\sin\left(\dfrac{\pi}{6}t\right) + 5\) models the height (in meters) of a point on a Ferris wheel, where \(t\) is time in seconds.

1. (a) State amplitude, midline, and period.  
2. (b) Find \(H(0)\) and interpret.  
3. (c) Find all \(t\) in \([0,12]\) when \(H(t)=5\).  
4. (d) Explain whether the wheel is moving clockwise or counterclockwise (given a graph).

**Annotated solution (sketch):**

- (a)  
  - Amplitude \(=3\), midline \(y=5\), period \(=\dfrac{2\pi}{\pi/6}=12\) seconds.

- (b)  
  - \(H(0)=3\sin 0 + 5 = 5\): starting at midline height 5 m.

- (c)  
  - \(H(t)=5 \Rightarrow 3\sin\left(\dfrac{\pi}{6}t\right)=0 \Rightarrow \sin\left(\dfrac{\pi}{6}t\right)=0\).  
  - So \(\dfrac{\pi}{6}t = n\pi \Rightarrow t = 6n\), \(n=0,1,2\).  
  - In \([0,12]\): \(t=0,6,12\).

- (d)  
  - Use graph orientation to justify direction (describe increasing/decreasing at \(t=0\)).

---

## 6. MCQ strategy & trap questions

### 6.1 High‑frequency MCQ concepts

- Interpreting graphs/tables of functions (increasing/decreasing, concavity, zeros, asymptotes).
- Matching functions to graphs (polynomial/rational/trig).
- Solving exponential/log equations.
- Trig values and transformations.
- Modeling interpretations (units, parameters, domain restrictions).

### 6.2 Graph reading speed‑run

When you see a graph:

1. **Mark key features:** intercepts, asymptotes, max/min, end behavior.
2. **Check monotonicity:** where increasing/decreasing.
3. **Check concavity:** where concave up/down.
4. **Relate to derivatives conceptually** (even though calculus isn’t tested, the language of “rate of change” appears).

### 6.3 Elimination strategies

- **Plug in simple values** (0, 1, easy angles) to test options.
- **Check units and domains**—many wrong answers violate context.
- **Compare end behavior** to eliminate mismatched polynomials/rationals.
- For trig, **check one full period** to see if amplitude/period match.

### 6.4 Classic traps

- **Domain traps:** including values where log or denominator is undefined.
- **Sign traps:** forgetting negative signs in transformations.
- **Period traps:** confusing \(B\) with period; period is \(\dfrac{2\pi}{|B|}\).
- **Model traps:** linear vs exponential vs sinusoidal—look at **constant difference vs constant ratio vs repeating pattern**.

---

## 7. Priority study matrix

Approximate priorities based on exam weighting and typical student difficulty.

| Topic                                      | Unit | Exam Weight | Difficulty (1–5) | Priority | Suggested Study Time (hrs) |
|-------------------------------------------|------|------------|------------------|----------|----------------------------|
| Polynomial end behavior & zeros           | 1    | High       | 3                | Very High | 8–10                     |
| Rational functions (asymptotes/holes)     | 1    | High       | 4                | Very High | 8–10                     |
| Polynomial/rational inequalities          | 1    | Medium     | 4                | High      | 5–7                      |
| Exponential models & equations            | 2    | High       | 3                | Very High | 8–10                     |
| Log properties & equations                | 2    | High       | 4                | Very High | 8–10                     |
| Semi‑log plots & data modeling            | 2    | Medium     | 3                | High      | 4–6                      |
| Unit circle & basic trig values           | 3    | High       | 3                | Very High | 8–10                     |
| Sinusoidal graphs & transformations       | 3    | High       | 4                | Very High | 8–10                     |
| Periodic modeling (FRQ style)             | 3    | High       | 4                | Very High | 8–10                     |
| Polar coordinates & graphs                | 3    | Medium     | 4                | High      | 5–7                      |
| Parametric, vectors, matrices (Unit 4)    | 4    | None       | 3–4              | Optional  | 0–6 (enrichment)         |

---

## 8. 8‑week study plan

Assume ~6–8 hours/week (more near the end).

### Week 1 – Foundations & Unit 1 basics

- **Topics:** power functions, rates of change, basic polynomials, zeros, multiplicity.
- **Hours:**  
  - 3 hrs content (notes + videos)  
  - 3 hrs practice (MCQ + short FRQ parts)
- **Checkpoint:** explain end behavior and multiplicity from a factored polynomial.

### Week 2 – Deep polynomial & rational functions

- **Topics:** full polynomial graphs, rational functions, asymptotes, holes, inequalities.
- **Practice:** 40–60 MCQ from Unit 1; 1–2 FRQ‑style modeling questions.
- **Checkpoint:** sketch a rational function from its equation and justify features.

### Week 3 – Exponentials & logs I

- **Topics:** sequences, exponential functions, growth/decay, basic log definitions.
- **Practice:** 40 MCQ; 1 FRQ on exponential modeling.
- **Checkpoint:** solve exponential equations and interpret parameters in context.

### Week 4 – Exponentials & logs II + semi‑log

- **Topics:** log properties, solving log equations/inequalities, semi‑log plots, model selection.
- **Practice:** 40 MCQ; 1 FRQ focusing on data modeling.
- **Checkpoint:** given data, choose and justify an exponential/log model.

### Week 5 – Trig basics & unit circle

- **Topics:** unit circle, trig functions, basic graphs, amplitude/period/phase shift.
- **Practice:** memorize key values; 40 MCQ; 1 FRQ on trig evaluation/graphs.
- **Checkpoint:** write a sinusoidal function from a graph or description.

### Week 6 – Periodic modeling & polar

- **Topics:** sinusoidal modeling, inverse trig, identities, polar coordinates & graphs.
- **Practice:** 40 MCQ; 1 FRQ on periodic modeling.
- **Checkpoint:** model a periodic context and interpret parameters.

### Week 7 – Mixed review + first full practice exam

- **Tasks:**
  - Take **one full practice exam** (AP Classroom or Barron’s).  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus/exam)  [Google Books](https://books.google.com/books/about/AP_Precalculus_Premium_2025_Prep_Book_wi.html?id=MYUMEQAAQBAJ)  
  - Review every missed question; categorize errors (content vs careless vs reading).
- **Checkpoint:** identify top 3 weak areas and plan targeted review.

### Week 8 – Targeted review + second practice exam

- **Tasks:**
  - 2–3 days of targeted drills on weak topics.
  - Take **another full practice exam** under timed conditions.
  - Final 2 days: light review, formula sheet, Desmos practice.

---

## 9. Best resources (current recommendations)

### 9.1 YouTube full courses & review

- **Math Teacher GOAT – AP Precalculus FULL COURSE & FULL LESSONS**  
  - Complete topic‑by‑topic coverage aligned to AP units.  [YouTube](https://www.youtube.com/playlist?list=PLNzd77h9IyBPeEXTEsD0ID-WOlDx6JN-p)  [YouTube](https://www.youtube.com/playlist?list=PLNzd77h9IyBOGeuUEyDaINK1G1yQ85Y-q)  
- **Michael Porinchak – AP Precalculus Full Course**  
  - Clear explanations, strong focus on exam‑style problems.  [YouTube](https://www.youtube.com/playlist?list=PL6334s8hsQG0M_I5RhCoIJiZWy5IF_pC4)  
- **MaPhy – AP Precalculus FRQ & MCQ**  
  - Great for targeted FRQ/MCQ practice.  [YouTube](https://www.youtube.com/playlist?list=PLCI1LaWjWlZ8rD2TictdYdmrh9CiMvgyA)  

### 9.2 Khan Academy

- Use **Precalculus** + **Get ready for Precalculus** for skill practice on polynomials, trig, vectors, matrices.  [Khan Academy](https://www.khanacademy.org/math/precalculus)  [Khan Academy](https://www.khanacademy.org/math/get-ready-for-precalculus)  
- Focus on:
  - Trig, rational functions, vectors, matrices, composite/inverse functions.

### 9.3 College Board AP Classroom

- **Official source** of AP‑style MCQ and FRQ with scoring guidelines.  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus)  [AP Central](https://apcentral.collegeboard.org/courses/ap-precalculus/exam)  
- Use:
  - Topic questions after each subtopic.
  - Progress checks at the end of each unit.
  - Released practice exams.

### 9.4 Prep books

- **Barron’s AP Precalculus Premium 2025**  
  - Very thorough content review, 3 practice tests, strong explanations.  [Google Books](https://books.google.com/books/about/AP_Precalculus_Premium_2025_Prep_Book_wi.html?id=MYUMEQAAQBAJ)  [Barnes & Noble](https://www.barnesandnoble.com/w/ap-precalculus-premium-2025-barrons-educational-series/1146537090)  
- **Princeton Review / 5 Steps to a 5**  
  - Typically more concise, strategy‑oriented; good as a **second resource**.
- General comparison: Barron’s often wins on **depth and explanations**, Princeton on **readability and pacing**.  [Test Prep Insight](https://testprepinsight.com/comparisons/barrons-vs-princeton-review/)  

### 9.5 Desmos activities

- Search **“Pre‑AP Calculus”** and **AP Precalculus** collections on Desmos Classroom for interactive modeling and graphing tasks.  [Desmos](https://www.desmos.com/calculator/mhtdlgqmdf)  [Desmos](https://www.desmos.com/calculator/jfahof0ezl)  

### 9.6 Anki & communities

- **Anki decks:**
  - Make your own for:
    - Unit circle values
    - Log rules
    - Key identities
    - Typical function forms
- **Communities:**
  - Reddit **r/APStudents** for exam discussion and motivation.
  - AP‑focused Discord servers for live help and accountability.

---

## 10. Exam day strategy

### 10.1 Time management

**Section I (MCQ):**

- Part A (28 Q / 80 min): ~2.8 min per question.
- Part B (12 Q / 40 min): ~3.3 min per question (but calculator‑heavy).

**Section II (FRQ):**

- 4 questions / 60 min → **15 min per FRQ**.
- Aim: 10–12 min answering, 3–5 min checking.

### 10.2 Approach to hard problems

- **MCQ:**
  - Spend at most ~3 minutes; if stuck, **mark and move on**.
  - Use elimination to guess intelligently if needed.
- **FRQ:**
  - Write **something** for each part—partial credit is huge.
  - If you can’t solve exactly, set up the correct equation or inequality and state what you would compute.

### 10.3 Writing clear FRQ responses

- Always:
  - Define variables clearly if you introduce them.
  - Use complete sentences for interpretations.
  - Include units in final answers.
  - Label graphs and tables if you sketch them.
- When using calculator:
  - State: “Using the graphing calculator, the solution is \(t\approx 3.27\).”

### 10.4 Night‑before & morning‑of

**Night‑before:**

- Light review only:
  - Formula sheet
  - Unit circle
  - 5–10 mixed MCQ
- No new topics. Sleep.

**Morning‑of:**

- Quick mental warm‑up:
  - 3–5 trig evaluations
  - 2 exponential/log equations
  - 1 quick modeling interpretation
- Check:
  - Calculator familiarity (if using a handheld in class; on exam you’ll use Bluebook Desmos).
  - Admission ticket, ID, etc.

---

If you want, next step I can:

- Turn this into a **printable 8‑week checklist**, or  
- Build **unit‑specific packets** (MCQ + FRQ) aligned to this guide.
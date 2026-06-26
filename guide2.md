# Calculus II — Complete Study Guide & Practice Exams

> **Final Exam Preparation Package** | Deep understanding over memorization

---

## Table of Contents
1. [Part 1 — Exam Analysis](#part-1--exam-analysis)
2. [Part 2 — Detailed Learning Guide](#part-2--detailed-learning-guide)
3. [Part 3 — Practice Exam A](#part-3--practice-exam-a)
4. [Part 4 — Practice Exam B](#part-4--practice-exam-b)
5. [Part 5 — Complete Solutions](#part-5--complete-solutions)

---

# PART 1 — EXAM ANALYSIS

## Topic Map by Problem

| # | Topic | Key Skill |
|---|-------|-----------|
| 1 | Product Rule + Evaluation at a Point | Apply product rule; evaluate at x=2 |
| 2 | Critical Points — Solving for Parameter | Set f'(x)=0; solve for a |
| 3 | Monotonicity (Increasing/Decreasing) | Sign analysis of f'(x) |
| 4 | Inflection Points — Solving for Parameter | Set f''(x)=0; solve for a |
| 5 | Separable ODEs | Separate variables; integrate both sides |
| 6 | Definite Integral (Area under curve) | Substitute and integrate |
| 7 | Volume of Revolution (Shell Method) | Shell method around Y-axis |
| 8 | Tangent Line to Curve | f'(x₀) gives slope; point-slope form |
| 9 | Integration by Parts | IBP formula; LIATE rule |
| 10 | Standard Indefinite Integrals | Integral table formulas |
| 11 | Level Curves & Tangent Line | Gradient; implicit differentiation |
| 12 | Gradient of f(x,y) | Partial derivatives at a point |
| 13 | Extrema of f(x,y) | Second derivative D-test |
| 14 | First-Order Linear ODE with IVP | Integrating factor method |
| 15 | Constrained Optimization | Area maximization; one-variable calculus |

## Key Themes

**Derivatives & Applications (P1–P4, P8):** Product rule, critical/inflection points, parameter-solving — ~4 problems. Know how to set derivatives to zero and solve for unknown parameters.

**Integration Techniques (P6, P9, P10):** Definite integrals, IBP, standard integral table. IBP is a guaranteed question. Memorize the formula and LIATE.

**Differential Equations (P5, P14):** Separable ODEs and first-order linear ODEs with integrating factors. Two ODE problems = high return on study time.

**Multivariable Calculus (P11–P13):** Gradient vectors, level curves, and extrema via D-test. Highest point value collectively.

**Geometric Applications (P7, P15):** Shell method and constrained optimization.

> 🎯 **Strategy:** Multivariable (P11–P13) and ODEs (P14) carry the most points. Master these first. Single-variable problems (P1–P10) are individually easier but numerous.

---

# PART 2 — DETAILED LEARNING GUIDE

---

## Problem 1 — Product Rule + Evaluation at a Point

### Problem Statement
$$\frac{d}{dx}\left[x^{1/5} \cdot h(x)\right]\bigg|_{x=2}, \quad h(2)=3,\quad h'(2)=-5$$

### Topic
Product Rule + Evaluation at a Point

### Theory & Formulas
**Product Rule:**
$$\frac{d}{dx}[f(x) \cdot g(x)] = f'(x) \cdot g(x) + f(x) \cdot g'(x)$$

Power rule for $x^{1/5}$:
$$\frac{d}{dx}\left[x^{1/5}\right] = \frac{1}{5}x^{-4/5}$$

### How to Recognize This Method
When you see a **product of two functions**, always apply the product rule — never differentiate just one factor.

### Step-by-Step Solution
**Step 1 — Apply product rule** with $f = x^{1/5}$, $g = h(x)$:
$$= \frac{1}{5}x^{-4/5} \cdot h(x) + x^{1/5} \cdot h'(x)$$

**Step 2 — Substitute** $x=2$, $h(2)=3$, $h'(2)=-5$:
$$= \frac{1}{5} \cdot 2^{-4/5} \cdot 3 + 2^{1/5} \cdot (-5)$$

**Step 3 — Simplify** (exact form):
$$= \frac{3}{5} \cdot 2^{-4/5} - 5 \cdot 2^{1/5} \approx 0.345 - 5.744 \approx -5.40$$

### Common Mistakes
- Forgetting to include BOTH terms of the product rule
- Sign error with $h'(2) = -5$
- Confusing $2^{1/5}$ (fifth root of 2) with $2/5$

### Exam Tip
If given numeric values for $h$ and $h'$, differentiate first, then substitute. Keep exact forms when possible.

---

## Problem 2 — Critical Points (Solving for a Parameter)

### Problem Statement
$$f(x) = ax^3 - 3x^2 + 4$$
Find $a$ such that $x = 3$ is an extremal (critical) point.

### Topic
Critical Points — Solving for a Parameter

### Theory & Formulas
A critical point occurs when $f'(c) = 0$.

### How to Recognize This Method
"Extremal point" = "critical point." Set $f'$ equal to zero at the given $x$-value, then solve for the unknown parameter.

### Step-by-Step Solution
**Step 1 — Differentiate:**
$$f'(x) = 3ax^2 - 6x$$

**Step 2 — Set $f'(3) = 0$:**
$$3a(9) - 6(3) = 0 \implies 27a - 18 = 0$$

**Step 3 — Solve:**
$$a = \frac{18}{27} = \frac{2}{3}$$

### Common Mistakes
- Confusing "extremal point" ($f'=0$) with "inflection point" ($f''=0$)
- Arithmetic errors computing $3a \cdot 3^2$

### Exam Tip
Always differentiate first, then plug in the given $x$. Never plug $x$ into $f(x)$ itself.

---

## Problem 3 — Monotonicity

### Problem Statement
Determine the intervals of increase and decrease of a given function $f(x)$.

### Topic
Monotonicity — Sign Analysis of $f'(x)$

### Theory & Formulas
- $f$ is **increasing** where $f'(x) > 0$
- $f$ is **decreasing** where $f'(x) < 0$

### How to Recognize This Method
Keywords: "increasing," "decreasing," "monotone," "ზრდადობა," "კლებადობა" → sign analysis of $f'$.

### Step-by-Step Solution (General Procedure)
**Step 1** — Find $f'(x)$.

**Step 2** — Solve $f'(x) = 0$ for critical points.

**Step 3** — Create a number line divided at critical points.

**Step 4** — Test a value in each interval.

**Example** with $f(x) = x^3 - 3x$: $f'(x) = 3x^2 - 3 = 3(x-1)(x+1)$

| Interval | Test value | $f'$ sign | Monotonicity |
|----------|-----------|-----------|-------------|
| $(-\infty,-1)$ | $x=-2$ | $+9 > 0$ | Increasing |
| $(-1, 1)$ | $x=0$ | $-3 < 0$ | Decreasing |
| $(1,+\infty)$ | $x=2$ | $+9 > 0$ | Increasing |

### Common Mistakes
- Confusing "$f$ is increasing" with "$f'$ is increasing"
- Missing a critical point and therefore an interval

### Exam Tip
Draw the number line explicitly with $+$ and $-$ signs. Easy to read, hard to get wrong.

---

## Problem 4 — Inflection Points (Solving for a Parameter)

### Problem Statement
$$f(x) = (2a-1)x^3 - 2x^2 + 1$$
Find $a$ such that $F(1,\, f(1))$ is an inflection point.

### Topic
Inflection Points — Solving for a Parameter

### Theory & Formulas
Inflection point at $x = c$ requires $f''(c) = 0$ (and concavity must change).

### How to Recognize This Method
"გადაღუნვის წერტილი" = inflection point → always use $f''(x) = 0$.

### Step-by-Step Solution
**Step 1 — Compute $f''(x)$:**
$$f'(x) = 3(2a-1)x^2 - 4x$$
$$f''(x) = 6(2a-1)x - 4$$

**Step 2 — Set $f''(1) = 0$:**
$$6(2a-1) - 4 = 0 \implies 12a - 6 - 4 = 0 \implies 12a = 10$$

**Step 3 — Solve:**
$$a = \frac{5}{6}$$

### Common Mistakes
- Confusing inflection ($f''=0$) with extremum ($f'=0$)
- Not verifying that concavity actually changes sign

### Exam Tip
Differentiate **twice**. Georgian exam: "გადაღუნვა" always means inflection.

---

## Problem 5 — Separable ODE

### Problem Statement
$$\frac{dy}{dx} = e^{2x - 3y}$$

### Topic
Separable Ordinary Differential Equations

### Theory & Formulas
Separable form: $\frac{dy}{dx} = f(x) \cdot g(y)$. Rewrite as:
$$\frac{1}{g(y)}\,dy = f(x)\,dx \quad \text{then integrate both sides}$$

Key identity: $e^{2x-3y} = e^{2x} \cdot e^{-3y}$

### How to Recognize This Method
Exponential ODE with both $x$ and $y$ in the exponent → separable. Use $e^{a+b} = e^a \cdot e^b$.

### Step-by-Step Solution
**Step 1 — Rewrite:**
$$\frac{dy}{dx} = e^{2x} \cdot e^{-3y}$$

**Step 2 — Separate:**
$$e^{3y}\,dy = e^{2x}\,dx$$

**Step 3 — Integrate:**
$$\frac{1}{3}e^{3y} = \frac{1}{2}e^{2x} + C$$

**Step 4 — Implicit solution:**
$$e^{3y} = \frac{3}{2}e^{2x} + C_1$$

**Explicit solution:**
$$y = \frac{1}{3}\ln\!\left[\frac{3}{2}e^{2x} + C_1\right]$$

### Common Mistakes
- Forgetting the constant of integration $C$
- Forgetting the $\frac{1}{3}$ factor when integrating $e^{3y}$
- Incorrect sign when dividing the exponential

### Exam Tip
After integrating, rename constants freely ($3C \to C$). Examiners usually accept implicit solutions.

---

## Problem 6 — Definite Integral (Area Under Curve)

### Problem Statement
Find the area bounded by $y = e^{2x}$, $x = 1$, $x = 2$, and the $x$-axis.

### Topic
Definite Integral — Area Under a Curve

### Theory & Formulas
$$A = \int_a^b f(x)\,dx \quad \text{when } f(x) \geq 0 \text{ on } [a,b]$$

For $e^{kx}$: $\displaystyle\int e^{kx}\,dx = \frac{1}{k}e^{kx} + C$

### How to Recognize This Method
"Area bounded by curve, two verticals, and $x$-axis" → definite integral with those limits.

### Step-by-Step Solution
**Step 1 — Confirm $f(x) \geq 0$:** Since $e^{(\cdot)} > 0$ always, yes.

**Step 2 — Set up and evaluate:**
$$A = \int_1^2 e^{2x}\,dx = \left[\frac{1}{2}e^{2x}\right]_1^2 = \frac{1}{2}(e^4 - e^2) \approx 23.6$$

### Common Mistakes
- Forgetting the $\frac{1}{2}$ from the substitution $u = 2x$
- Mixing up limits after substitution

### Exam Tip
For $\int e^{kx}\,dx$, the antiderivative is always $\frac{1}{k}e^{kx}$. Memorize this.

---

## Problem 7 — Volume of Revolution (Shell Method)

### Problem Statement
The region bounded by $y = \sqrt{x}$, the $x$-axis, and $x = 2$ rotates around the $Y$-axis. Find the volume.

### Topic
Shell Method — Rotation around the Y-axis

### Theory & Formulas
**Shell Method** (rotation around $Y$-axis):
$$V = 2\pi \int_a^b x \cdot f(x)\,dx$$

### How to Recognize This Method
Rotation around the $Y$-axis (not $X$-axis) → use the **shell method**, integrate with respect to $x$.

### Step-by-Step Solution
$$V = 2\pi \int_0^2 x \cdot \sqrt{x}\,dx = 2\pi \int_0^2 x^{3/2}\,dx$$

$$= 2\pi \left[\frac{x^{5/2}}{5/2}\right]_0^2 = 2\pi \cdot \frac{2}{5} \cdot 2^{5/2} = \frac{4\pi}{5} \cdot 4\sqrt{2} = \frac{16\pi\sqrt{2}}{5}$$

### Common Mistakes
- Using disk/washer method (for $X$-axis rotation) when it's $Y$-axis
- Forgetting the $2\pi$ factor
- Confusing volume and surface area formulas

### Exam Tip
Y-axis rotation → immediately write $V = 2\pi\int x \cdot f(x)\,dx$ before doing anything else.

---

## Problem 8 — Tangent Line to a Curve

### Problem Statement
Find the tangent line to $y = 4e^{x-2} + 2x - 3$ at the point $(2,\, 5)$.

### Topic
Tangent Line at a Given Point

### Theory & Formulas
Tangent line at $(x_0, y_0)$:
$$y - y_0 = f'(x_0)(x - x_0)$$

### How to Recognize This Method
"Tangent line at point $(a,b)$" → evaluate $f'$ at $x=a$, write point-slope equation.

### Step-by-Step Solution
**Step 1 — Verify** $(2,5)$ is on the curve:
$$y(2) = 4e^0 + 4 - 3 = 4 + 4 - 3 = 5\checkmark$$

**Step 2 — Differentiate:**
$$f'(x) = 4e^{x-2} + 2$$

**Step 3 — Evaluate at $x=2$:**
$$f'(2) = 4e^0 + 2 = 6 \quad (m = 6)$$

**Step 4 — Write tangent line:**
$$y - 5 = 6(x-2) \implies \boxed{y = 6x - 7}$$

### Common Mistakes
- Using the $y$-value instead of the slope from $f'$
- Forgetting chain rule when the exponent has a coefficient

### Exam Tip
Always verify the point lies on the curve first. If it doesn't, you've misread the problem.

---

## Problem 9 — Integration by Parts

### Problem Statement
$$\int x\cos(2x)\,dx \quad \text{(by integration by parts)}$$

### Topic
Integration by Parts (IBP)

### Theory & Formulas
$$\int u\,dv = uv - \int v\,du$$

**LIATE Rule** (priority for choosing $u$): **L**ogarithm, **I**nverse trig, **A**lgebraic, **T**rig, **E**xponential

### How to Recognize This Method
Product of polynomial × trig/exponential → IBP. "ნაწილობრივი ინტეგრირება" = IBP.

### Step-by-Step Solution
**Step 1 — Assign:**
$$u = x, \quad dv = \cos(2x)\,dx$$
$$du = dx, \quad v = \frac{\sin(2x)}{2}$$

**Step 2 — Apply IBP:**
$$\int x\cos(2x)\,dx = \frac{x\sin(2x)}{2} - \int \frac{\sin(2x)}{2}\,dx$$

**Step 3 — Evaluate remaining integral:**
$$\int \frac{\sin(2x)}{2}\,dx = -\frac{\cos(2x)}{4}$$

**Step 4 — Combine:**
$$= \frac{x\sin(2x)}{2} + \frac{\cos(2x)}{4} + C$$

### Common Mistakes
- Choosing $u = \cos(2x)$ (makes things harder)
- Forgetting $\frac{1}{2}$ when integrating $\cos(2x)$
- Sign error: $\int\sin(2x)\,dx = -\frac{\cos(2x)}{2}$

### Exam Tip
Memorize: $\int\cos(kx)\,dx = \frac{\sin(kx)}{k}$ and $\int\sin(kx)\,dx = -\frac{\cos(kx)}{k}$. The $\frac{1}{k}$ factor is critical.

---

## Problem 10 — Standard Indefinite Integrals

### Problem Statement
$$\int \left(\frac{5}{x} - 3\cdot 4^x + \frac{7}{3x^2} - 4\sin x\right)dx$$

### Topic
Standard Indefinite Integrals (Term by Term)

### Theory & Formulas
| Integrand | Antiderivative |
|-----------|---------------|
| $1/x$ | $\ln\|x\| + C$ |
| $a^x$ | $a^x/\ln a + C$ |
| $x^n$ $(n\neq -1)$ | $x^{n+1}/(n+1) + C$ |
| $\sin x$ | $-\cos x + C$ |
| $\cos x$ | $\sin x + C$ |

### Step-by-Step Solution
$$\int \frac{5}{x}\,dx = 5\ln|x|$$
$$\int -3\cdot 4^x\,dx = -\frac{3\cdot 4^x}{\ln 4}$$
$$\int \frac{7}{3x^2}\,dx = \frac{7}{3}\int x^{-2}\,dx = \frac{7}{3}\cdot\frac{x^{-1}}{-1} = -\frac{7}{3x}$$
$$\int -4\sin x\,dx = 4\cos x$$

**Full answer:**
$$= 5\ln|x| - \frac{3\cdot 4^x}{\ln 4} - \frac{7}{3x} + 4\cos x + C$$

### Common Mistakes
- Writing $\int 4^x\,dx = 4^x$ (missing $\div\ln 4$)
- $\int x^{-2}\,dx = x^{-1}/(-1)$, not $x^{-1}/1$
- $\int\sin x\,dx = -\cos x$, not $+\cos x$

### Exam Tip
Write all formulas on your scratch paper before starting. Speed comes from a memorized table.

---

## Problem 11 — Level Curves & Tangent Line

### Problem Statement
Given $f(x,y) = \sqrt{x^2+y^2+3}$. The level curve is $f(x,y) = \sqrt{5}$. Find the tangent line at a given point.

### Topic
Level Curves and Implicit Tangent Lines

### Theory & Formulas
For level curve $F(x,y) = c$, the tangent line at $(x_0, y_0)$:
$$F_x(x_0,y_0)(x-x_0) + F_y(x_0,y_0)(y-y_0) = 0$$

The gradient $\nabla F$ is **perpendicular** to the level curve.

### How to Recognize This Method
"Level curve" + "tangent line" → compute partial derivatives, form gradient equation at the point.

### Step-by-Step Solution (at point $(1,1)$)
**Step 1 — Find level curve:**
$$\sqrt{x^2+y^2+3} = \sqrt{5} \implies x^2 + y^2 = 2$$

**Step 2 — Partial derivatives of** $F = x^2+y^2$:
$$F_x = 2x, \quad F_y = 2y$$

**Step 3 — At $(1,1)$:** (check: $1+1=2$ ✓)
$$\nabla F(1,1) = (2,\,2)$$

**Step 4 — Tangent line:**
$$2(x-1) + 2(y-1) = 0 \implies \boxed{x + y = 2}$$

### Common Mistakes
- Confusing the gradient (normal direction) with the tangent direction
- Using the wrong $F$ — differentiate the *implicit* expression, not $f$ itself

### Exam Tip
For any level curve $F(x,y)=c$: tangent = $F_x(x-x_0) + F_y(y-y_0) = 0$. Write this formula down first.

---

## Problem 12 — Gradient of f(x,y)

### Problem Statement
$$f(x,y) = x^3y^2 - 2xy + 3 \quad \text{Find } \nabla f \text{ at } (2,\,2)$$

### Topic
Gradient of a Multivariable Function

### Theory & Formulas
$$\nabla f = \left(\frac{\partial f}{\partial x},\; \frac{\partial f}{\partial y}\right)$$

When computing $\partial f/\partial x$: treat $y$ as constant. When computing $\partial f/\partial y$: treat $x$ as constant.

### Step-by-Step Solution
**Step 1 — $f_x$ (treat $y$ as constant):**
$$f_x = 3x^2y^2 - 2y$$

**Step 2 — $f_y$ (treat $x$ as constant):**
$$f_y = 2x^3y - 2x$$

**Step 3 — Evaluate at $(2,2)$:**
$$f_x(2,2) = 3(4)(4) - 2(2) = 48 - 4 = 44$$
$$f_y(2,2) = 2(8)(2) - 2(2) = 32 - 4 = 28$$

$$\boxed{\nabla f(2,2) = (44,\; 28)}$$

### Common Mistakes
- Differentiating $y$-terms when finding $f_x$
- Arithmetic errors: $3 \cdot 2^2 \cdot 2^2 = 3 \cdot 4 \cdot 4 = 48$

### Exam Tip
Write "treat $y$ as constant" and "treat $x$ as constant" explicitly. Prevents variable mix-ups under pressure.

---

## Problem 13 — Extrema of f(x,y)

### Problem Statement
$$f(x,y) = xy - x^2 - y^2 - 2x - 2y + 4 \quad \text{Find extreme values}$$

### Topic
Extrema of f(x,y) — Second Derivative (D) Test

### Theory & Formulas
**Process:**
1. Find critical points: solve $f_x = 0$ AND $f_y = 0$ simultaneously
2. Compute discriminant: $D = f_{xx}\,f_{yy} - (f_{xy})^2$

| Condition | Conclusion |
|-----------|-----------|
| $D > 0$ and $f_{xx} < 0$ | Local maximum |
| $D > 0$ and $f_{xx} > 0$ | Local minimum |
| $D < 0$ | Saddle point |
| $D = 0$ | Inconclusive |

### Step-by-Step Solution
**Step 1 — Partial derivatives:**
$$f_x = y - 2x - 2 = 0$$
$$f_y = x - 2y - 2 = 0$$

**Step 2 — Solve the system:**
From $f_x = 0$: $y = 2x + 2$

Substitute into $f_y = 0$:
$$x - 2(2x+2) - 2 = 0 \implies -3x - 6 = 0 \implies x = -2,\; y = -2$$

**Step 3 — Second partials:**
$$f_{xx} = -2, \quad f_{yy} = -2, \quad f_{xy} = 1$$

**Step 4 — Compute D:**
$$D = (-2)(-2) - (1)^2 = 4 - 1 = 3 > 0$$

$D > 0$ and $f_{xx} = -2 < 0$ → **local maximum** at $(-2,-2)$.

**Step 5 — Compute maximum value:**
$$f(-2,-2) = 4 - 4 - 4 + 4 + 4 + 4 = \boxed{8}$$

### Common Mistakes
- Writing $D = f_{xx}f_{yy} - f_{xy}$ instead of $D = f_{xx}f_{yy} - (f_{xy})^2$
- Not checking sign of $f_{xx}$ after confirming $D > 0$
- Substitution errors when solving the system

### Exam Tip
Circle the $D$ formula. It's easy to forget the **square** on $f_{xy}$ under exam pressure.

---

## Problem 14 — First-Order Linear ODE with IVP

### Problem Statement
$$\frac{dy}{dx} + \frac{3}{x}\,y = x, \quad x > 0, \quad y(1) = -2$$

### Topic
First-Order Linear ODE — Integrating Factor Method

### Theory & Formulas
Standard form: $y' + P(x)\,y = Q(x)$

Integrating factor: $\mu(x) = e^{\int P(x)\,dx}$

Then: $\frac{d}{dx}[\mu\,y] = \mu\,Q(x)$ — integrate both sides.

### Step-by-Step Solution
**Step 1 — Identify:** $P(x) = 3/x$, $Q(x) = x$

**Step 2 — Compute $\mu$:**
$$\mu(x) = e^{\int 3/x\,dx} = e^{3\ln x} = x^3$$

**Step 3 — Multiply both sides by $x^3$:**
$$x^3y' + 3x^2y = x^4 \implies \frac{d}{dx}\!\left[x^3 y\right] = x^4$$

**Step 4 — Integrate:**
$$x^3 y = \int x^4\,dx = \frac{x^5}{5} + C$$

**Step 5 — Solve for $y$:**
$$y = \frac{x^2}{5} + \frac{C}{x^3}$$

**Step 6 — Apply $y(1) = -2$:**
$$-2 = \frac{1}{5} + C \implies C = -\frac{11}{5}$$

$$\boxed{y = \frac{x^2}{5} - \frac{11}{5x^3}}$$

### Common Mistakes
- Not multiplying EVERY term by the integrating factor
- Not recognizing $e^{3\ln x} = x^3$
- Applying IVP before dividing by $\mu$

### Exam Tip
After multiplying by $\mu$, the left side **always** becomes $\frac{d}{dx}[\mu\,y]$. Verify this before integrating.

---

## Problem 15 — Constrained Optimization

### Problem Statement
Rectangle inscribed in a right triangle with legs 2 and 3. Constraint: $(3-x)/3 = y/2$. Maximize area.

### Topic
Constrained Optimization — Maximize Area

### Theory & Formulas
Express area as a function of **one** variable using the constraint, then maximize by setting $S'(x) = 0$.

### Step-by-Step Solution
**Step 1 — Extract $y$ from constraint:**
$$y = \frac{2}{3}(3-x)$$

**Step 2 — Area function:**
$$S(x) = x \cdot y = \frac{2}{3}(3x - x^2)$$

**Step 3 — Differentiate:**
$$S'(x) = \frac{2}{3}(3 - 2x)$$

**Step 4 — Set $S'(x) = 0$:**
$$3 - 2x = 0 \implies x = \frac{3}{2}$$

**Step 5 — Find $y$ and $S_{\max}$:**
$$y = \frac{2}{3}\!\left(3 - \frac{3}{2}\right) = 1, \quad S_{\max} = \frac{3}{2}$$

**Verify:** $S''(x) = -\frac{4}{3} < 0$ → maximum ✓

### Common Mistakes
- Confusing area of triangle with area of rectangle ($S = x \cdot y$)
- Not verifying maximum ($S'' < 0$) vs minimum

### Exam Tip
Always verify max vs min with the second derivative or boundary values.

---

# PART 3 — PRACTICE EXAM A

**15 Questions · Total: 25 Points**
*Instructions: Show all work. Partial credit awarded for correct method.*

---

**Q1 [1 pt]**
Differentiate $f(x) = \sqrt[3]{x} \cdot g(x)$ at $x = 8$, given $g(8) = 4$ and $g'(8) = -3$.

---

**Q2 [1 pt]**
Find the value of $b$ such that $x = 2$ is a critical point of $f(x) = bx^3 - 12x + 5$.

---

**Q3 [1 pt]**
Find the intervals of increase and decrease of $f(x) = x^3 - 6x^2 + 9x$.

---

**Q4 [1 pt]**
Find $a$ so that $x = 2$ is an inflection point of $f(x) = (3a-2)x^3 - 6x^2 + 1$.

---

**Q5 [1 pt]**
Solve the separable ODE:
$$\frac{dy}{dx} = e^{3x - 2y}$$

---

**Q6 [1 pt]**
Find the area bounded by $y = e^{3x}$, $x = 0$, $x = 1$, and the $x$-axis.

---

**Q7 [1 pt]**
The region bounded by $y = x^2$, the $x$-axis, and $x = 3$ rotates around the $Y$-axis. Find the volume.

---

**Q8 [1 pt]**
Find the tangent line to $y = 3e^{x-1} + 4x - 2$ at $(1,\, 5)$.

---

**Q9 [1 pt]**
Compute $\displaystyle\int x\,e^{2x}\,dx$ using integration by parts.

---

**Q10 [1 pt]**
Compute:
$$\int\!\left(\frac{3}{x} + 2\cdot 3^x - \frac{5}{2x^3} + 6\cos x\right)dx$$

---

**Q11 [4 pts]**
Given $f(x,y) = \sqrt{x^2+y^2+7}$. The level curve is $f(x,y) = \sqrt{11}$. Find the tangent line to this level curve at $(1,\,1)$.

---

**Q12 [4 pts]**
Find $\nabla f$ at $(1,\,2)$ for $f(x,y) = x^2y^3 - 3x^2y + 5$.

---

**Q13 [4 pts]**
Find the extreme values of $f(x,y) = 2xy - x^2 - 2y^2 + 4x$.

---

**Q14 [4 pts]**
Solve:
$$\frac{dy}{dx} + \frac{2}{x}\,y = x^2, \quad x > 0, \quad y(1) = 1$$

---

**Q15 [4 pts]**
Maximize the area of a rectangle inscribed in a right triangle with legs 3 and 4. Use constraint $(4-x)/4 = y/3$.

---

# PART 4 — PRACTICE EXAM B

**15 Questions · Total: 25 Points**
*Instructions: Show all work. Partial credit awarded for correct method.*

---

**Q1 [1 pt]**
Differentiate $h(x) = x^{1/4} \cdot k(x)$ at $x = 16$, given $k(16) = 5$ and $k'(16) = -2$.

---

**Q2 [1 pt]**
Find $c$ such that $x = -1$ is a critical point of $f(x) = cx^3 + 6x^2 - 3$.

---

**Q3 [1 pt]**
Determine the monotone intervals of $f(x) = 2x^3 - 3x^2 - 12x + 1$.

---

**Q4 [1 pt]**
Find $k$ so that $x = 1$ is an inflection point of $f(x) = (k+1)x^3 - 3x^2 + 2$.

---

**Q5 [1 pt]**
Solve:
$$\frac{dy}{dx} = e^{x - 4y}$$

---

**Q6 [1 pt]**
Find the area under $y = e^{2x}$ from $x = 1$ to $x = 3$.

---

**Q7 [1 pt]**
The region bounded by $y = \sqrt{x}$, the $x$-axis, and $x = 4$ rotates about the $Y$-axis. Find the volume.

---

**Q8 [1 pt]**
Find the tangent to $y = 2e^{x-3} + 3x - 5$ at $(3,\, 4)$.

---

**Q9 [1 pt]**
Compute $\displaystyle\int x\sin(3x)\,dx$ using IBP.

---

**Q10 [1 pt]**
Compute:
$$\int\!\left(\frac{4}{x} - 5^x + \frac{8}{3x^2} - 7\sin x\right)dx$$

---

**Q11 [4 pts]**
Given $f(x,y) = \sqrt{2x^2+y^2+3}$. Level curve $f = \sqrt{7}$. Find the tangent at $(1,\,\sqrt{2})$.

---

**Q12 [4 pts]**
Find $\nabla f$ at $(2,\,1)$ for $f(x,y) = x^2y - 3xy^2 + 2$.

---

**Q13 [4 pts]**
Find the extreme values of $f(x,y) = x^2 + y^2 - 2x - 4y + 8$.

---

**Q14 [4 pts]**
Solve:
$$\frac{dy}{dx} - \frac{2}{x}\,y = x^3, \quad x > 0, \quad y(1) = 0$$

---

**Q15 [4 pts]**
Maximize the area of a rectangle with one side on the $x$-axis and an upper vertex on $y = -\frac{2}{3}x + 4$ (first quadrant).

---

# PART 5 — COMPLETE SOLUTIONS

---

## Original Exam — Solutions

### P1
$$\frac{d}{dx}\left[x^{1/5}h(x)\right]\bigg|_{x=2} = \frac{1}{5}x^{-4/5}h(x)+x^{1/5}h'(x)\bigg|_{x=2}$$
$$= \frac{3}{5}\cdot 2^{-4/5} - 5\cdot 2^{1/5} \approx 0.345 - 5.744 \approx \mathbf{-5.40}$$

### P2
$f'(x) = 3ax^2 - 6x$. Set $f'(3)=0$: $27a - 18 = 0 \Rightarrow \boxed{a = 2/3}$

### P3
General procedure: find $f'(x)$, set to zero for critical points, test sign in each interval. $f'>0$ = increasing; $f'<0$ = decreasing.

### P4
$f''(x) = 6(2a-1)x - 4$. Set $f''(1)=0$: $6(2a-1)-4=0 \Rightarrow 12a=10 \Rightarrow \boxed{a = 5/6}$

### P5
Separate: $e^{3y}dy = e^{2x}dx$. Integrate: $\frac{1}{3}e^{3y} = \frac{1}{2}e^{2x}+C$.
$$\boxed{e^{3y} = \frac{3}{2}e^{2x} + C_1}$$

### P6
$$A = \int_1^2 e^{2x}\,dx = \left[\frac{e^{2x}}{2}\right]_1^2 = \frac{e^4-e^2}{2} \approx \mathbf{23.6}$$

### P7
Shell method: $V = 2\pi\int_0^2 x\sqrt{x}\,dx = 2\pi\left[\frac{x^{5/2}}{5/2}\right]_0^2 = \dfrac{16\pi\sqrt{2}}{5}$

### P8
$f'(x) = 4e^{x-2}+2$. $f'(2)=6$. Tangent: $\boxed{y = 6x - 7}$

### P9
$u=x$, $dv=\cos(2x)dx$, $v=\sin(2x)/2$.
$$\int x\cos(2x)\,dx = \frac{x\sin(2x)}{2} + \frac{\cos(2x)}{4} + C$$

### P10
$$5\ln|x| - \frac{3\cdot 4^x}{\ln 4} - \frac{7}{3x} + 4\cos x + C$$

### P11
Level curve: $x^2+y^2=2$. At $(1,1)$: $\nabla F = (2,2)$. Tangent: $\boxed{x+y=2}$

### P12
$f_x = 3x^2y^2-2y$; $f_x(2,2)=44$. $f_y = 2x^3y-2x$; $f_y(2,2)=28$. $\boxed{\nabla f = (44,28)}$

### P13
Critical point: $x=-2, y=-2$. $D = (-2)(-2)-(1)^2 = 3 > 0$, $f_{xx}<0$ → **local max**: $\boxed{f(-2,-2)=8}$

### P14
$\mu = x^3$. $x^3y = x^5/5+C$. $y(1)=-2$: $C=-11/5$. $\boxed{y = x^2/5 - 11/(5x^3)}$

### P15
$y = \frac{2}{3}(3-x)$. $S=\frac{2}{3}(3x-x^2)$. $S'=0 \Rightarrow x=3/2$, $y=1$. $\boxed{S_{\max}=3/2}$

---

## Practice Exam A — Solutions

### A-Q1
Product rule: $\frac{1}{3}x^{-2/3}g(x)+x^{1/3}g'(x)\big|_{x=8}$
$= \frac{1}{3}(8^{-2/3})(4) + 8^{1/3}(-3) = \frac{1}{3}\cdot\frac{1}{4}\cdot 4 + 2(-3) = \frac{1}{3} - 6 = -\frac{17}{3}$

### A-Q2
$f'(x)=3bx^2-12$. $f'(2)=12b-12=0 \Rightarrow \boxed{b=1}$

### A-Q3
$f'(x)=3x^2-12x+9=3(x-1)(x-3)$. Decreasing on $(1,3)$; increasing on $(-\infty,1)\cup(3,+\infty)$.

### A-Q4
$f''(x)=6(3a-2)x-12$. $f''(2)=12(3a-2)-12=0 \Rightarrow 36a=36 \Rightarrow \boxed{a=1}$

### A-Q5
$e^{2y}dy=e^{3x}dx$. $\frac{1}{2}e^{2y}=\frac{1}{3}e^{3x}+C$. $\boxed{e^{2y}=\frac{2}{3}e^{3x}+C_1}$

### A-Q6
$$\int_0^1 e^{3x}\,dx = \left[\frac{e^{3x}}{3}\right]_0^1 = \frac{e^3-1}{3}$$

### A-Q7
Shell: $V=2\pi\int_0^3 x\cdot x^2\,dx = 2\pi\left[\frac{x^4}{4}\right]_0^3 = 2\pi\cdot\frac{81}{4} = \dfrac{81\pi}{2}$

### A-Q8
$f'(x)=3e^{x-1}+4$. $f'(1)=3+4=7$. Tangent: $\boxed{y=7x-2}$

### A-Q9
$u=x$, $dv=e^{2x}dx$, $v=e^{2x}/2$.
$$\int xe^{2x}dx = \frac{x}{2}e^{2x} - \frac{1}{4}e^{2x} + C$$

### A-Q10
$$3\ln|x| + \frac{2\cdot 3^x}{\ln 3} + \frac{5}{4x^2} + 6\sin x + C$$

### A-Q11
Level curve: $x^2+y^2=4$. At $(1,1)$: $F_x=2,F_y=2$. Tangent: $\boxed{x+y=2}$

### A-Q12
$f_x=2xy^3-6xy$; $f_x(1,2)=2(1)(8)-6(1)(2)=16-12=4$.
$f_y=3x^2y^2-3x^2$; $f_y(1,2)=3(1)(4)-3(1)=9$.
$\boxed{\nabla f=(4,9)}$

### A-Q13
$f_x=2y-2x+4=0$, $f_y=2x-4y=0 \Rightarrow x=2y$. Substitute: $2y-4y+4=0 \Rightarrow y=2,\,x=4$.
$f_{xx}=-2,f_{yy}=-4,f_{xy}=2$. $D=8-4=4>0$, $f_{xx}<0$ → **local max** at $(4,2)$.

### A-Q14
$\mu=x^2$. $d/dx[x^2y]=x^4$. $x^2y=x^5/5+C$. $y(1)=1$: $C=4/5$.
$$\boxed{y = \frac{x^3}{5} + \frac{4}{5x^2}}$$

### A-Q15
$y=\frac{3}{4}(4-x)$. $S=\frac{3}{4}(4x-x^2)$. $S'=0\Rightarrow x=2,\,y=3/2$. $\boxed{S_{\max}=3}$

---

## Practice Exam B — Solutions

### B-Q1
$\frac{1}{4}x^{-3/4}k(x)+x^{1/4}k'(x)\big|_{x=16}$
$=\frac{1}{4}(16^{-3/4})(5)+16^{1/4}(-2)=\frac{1}{4}\cdot\frac{1}{8}\cdot 5+2(-2)=\frac{5}{32}-4$

### B-Q2
$f'(x)=3cx^2+12x$. $f'(-1)=3c-12=0 \Rightarrow \boxed{c=4}$

### B-Q3
$f'=6x^2-6x-12=6(x-2)(x+1)$. Increasing: $(-\infty,-1)\cup(2,+\infty)$. Decreasing: $(-1,2)$.

### B-Q4
$f''(x)=6(k+1)x-6$. $f''(1)=6(k+1)-6=0 \Rightarrow \boxed{k=0}$

### B-Q5
$e^{4y}dy=e^x dx$. $\frac{1}{4}e^{4y}=e^x+C$. $\boxed{e^{4y}=4e^x+C_1}$

### B-Q6
$$\int_1^3 e^{2x}\,dx = \left[\frac{e^{2x}}{2}\right]_1^3 = \frac{e^6-e^2}{2}$$

### B-Q7
Shell: $V=2\pi\int_0^4 x\sqrt{x}\,dx=2\pi\left[\frac{x^{5/2}}{5/2}\right]_0^4=2\pi\cdot\frac{2}{5}\cdot 32=\dfrac{128\pi}{5}$

### B-Q8
$f'(x)=2e^{x-3}+3$. $f'(3)=2+3=5$. Tangent: $\boxed{y=5x-11}$

### B-Q9
$u=x$, $dv=\sin(3x)dx$, $v=-\cos(3x)/3$.
$$\int x\sin(3x)\,dx = -\frac{x\cos(3x)}{3} + \frac{\sin(3x)}{9} + C$$

### B-Q10
$$4\ln|x| - \frac{5^x}{\ln 5} - \frac{8}{3x} + 7\cos x + C$$

### B-Q11
Level curve: $2x^2+y^2=4$. At $(1,\sqrt{2})$: $F_x=4x=4$, $F_y=2y=2\sqrt{2}$.
Tangent: $4(x-1)+2\sqrt{2}(y-\sqrt{2})=0 \Rightarrow 4x+2\sqrt{2}\,y=8 \Rightarrow \boxed{2x+\sqrt{2}\,y=4}$

### B-Q12
$f_x=2xy-3y^2$; $f_x(2,1)=4-3=1$.
$f_y=x^2-6xy$; $f_y(2,1)=4-12=-8$.
$\boxed{\nabla f=(1,-8)}$

### B-Q13
$f_x=2x-2=0\Rightarrow x=1$. $f_y=2y-4=0\Rightarrow y=2$.
$f_{xx}=2,f_{yy}=2,f_{xy}=0$. $D=4>0$, $f_{xx}>0$ → **local minimum**: $\boxed{f(1,2)=3}$

### B-Q14
$\mu=e^{-2\ln x}=1/x^2$. $d/dx[y/x^2]=x$. $y/x^2=x^2/2+C$.
$y(1)=0$: $1/2+C=0\Rightarrow C=-1/2$.
$$\boxed{y = \frac{x^4}{2} - \frac{x^2}{2}}$$

### B-Q15
$y=-\frac{2}{3}x+4$. $S=x\!\left(-\frac{2}{3}x+4\right)=-\frac{2}{3}x^2+4x$.
$S'=-\frac{4}{3}x+4=0\Rightarrow x=3,\,y=2$. $\boxed{S_{\max}=6}$

---

*Good luck on the exam! Focus on understanding the method, not just the answer.*

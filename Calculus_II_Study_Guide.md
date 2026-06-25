# Calculus II — Final Exam: Complete Study & Practice Guide

> Exam analysis · Detailed learning guide · Two full practice exams · Worked solutions
> Prepared for an intensive 2-day review.
> **Topics:** differentiation · integration · differential equations · multivariable calculus

**Contents**

1. [Part 1 — Exam Analysis](#part-1--exam-analysis)
2. [Part 2 — Detailed Learning Guide](#part-2--detailed-learning-guide)
3. [Part 3 — Practice Exam A](#part-3--practice-exam-a)
4. [Part 4 — Practice Exam B](#part-4--practice-exam-b)
5. [Part 5 — Complete Solutions](#part-5--complete-solutions)

---

## Part 1 — Exam Analysis

This exam is a broad Calculus II final. It samples three big themes: **(a)** single-variable differential calculus used to analyze functions (slopes, extrema, concavity), **(b)** integral calculus and its applications (antiderivatives, area, volume), and **(c)** the bridge into differential equations and multivariable calculus (separable and linear ODEs, gradients, level curves, and optimization). The first ten questions are short, single-skill items worth 1 point each; the last five are multi-step problems worth 4 points each.

### What each question tests

| # | Topic tested | Skill required |
|---|--------------|----------------|
| 1 | Differentiation: product + power/root rule | Differentiate $\sqrt[5]{x}\,h(x)$ and evaluate at a point |
| 2 | Critical points with a parameter | Use $f'(x_0)=0$ to solve for the constant $a$ |
| 3 | Monotonicity (increase / decrease) | Sign analysis of $f'(x)$ on a number line |
| 4 | Inflection points with a parameter | Use $f''(x_0)=0$ to solve for $a$ |
| 5 | Separable differential equation | Separate variables, integrate both sides |
| 6 | Area under a curve | Set up and evaluate a definite integral |
| 7 | Volume of a solid of revolution | Shell / disk method about the $y$-axis |
| 8 | Tangent line to a curve | Use $y-y_0=f'(x_0)(x-x_0)$ |
| 9 | Integration by parts | Apply $\int u\,dv = uv-\int v\,du$ |
| 10 | Indefinite integral (basic rules) | Antiderivatives of $1/x$, $a^x$, powers, $\sin x$ |
| 11 | Level curves & tangent line | Gradient is normal to the level curve |
| 12 | Gradient of $f(x,y)$ | Compute partials $f_x,f_y$ and evaluate |
| 13 | Extrema of $f(x,y)$ | Solve $\nabla f=0$, apply the Hessian test |
| 14 | First-order linear ODE (IVP) | Integrating-factor method + initial condition |
| 15 | Applied optimization | One-variable model, maximize with $S'=0$ |

### Recurring patterns, formulas & techniques

- **Critical-point machinery dominates.** Three different questions reduce to “set a derivative to zero”: $f'=0$ for extrema (Q2), $f''=0$ for inflection (Q4), and $\nabla f=0$ for surfaces (Q13). Recognize them as the *same idea* applied to first / second / partial derivatives.
- **Core differentiation rules:** product rule $(uv)'=u'v+uv'$, power rule $\dfrac{d}{dx}x^n=nx^{n-1}$ (roots are fractional powers), chain rule, and $\dfrac{d}{dx}e^{g(x)}=g'(x)e^{g(x)}$.
- **Core integration rules:**

$$\int x^n\,dx=\frac{x^{n+1}}{n+1},\quad \int \frac{1}{x}\,dx=\ln|x|,\quad \int a^x\,dx=\frac{a^x}{\ln a},\quad \int \sin x\,dx=-\cos x,\quad \int e^{kx}\,dx=\frac{1}{k}e^{kx}.$$

- **Integration by parts:** $\displaystyle\int u\,dv = uv-\int v\,du$, with **LIATE** for choosing $u$.
- **Applications of the integral:** area $=\displaystyle\int_a^b f(x)\,dx$; volume about the $y$-axis by shells $V=\displaystyle\int_a^b 2\pi x\,f(x)\,dx$.
- **Differential equations:** separable form $\dfrac{dy}{dx}=g(x)h(y)$, and first-order linear form $\dfrac{dy}{dx}+P(x)y=Q(x)$ solved by the integrating factor $\mu=e^{\int P\,dx}$.
- **Multivariable toolkit:** partial derivatives, the gradient $\nabla f=(f_x,f_y)$, the fact that $\nabla f \perp$ level curves, and the Hessian discriminant $D=f_{xx}f_{yy}-f_{xy}^2$.

### What matters most (next 48 hours)

1. **Master “derivative = 0” problems.** Be fluent moving between $f'=0$, $f''=0$, and $\nabla f=0$. This single idea covers Q2, Q3, Q4, Q13 and half of Q15.
2. **Drill the integration table** plus integration by parts. Q9 and Q10 are guaranteed points if your antiderivatives are automatic.
3. **Know the two ODE recipes cold:** separation of variables and the integrating factor (Q5, Q14).
4. **Practice the second-derivative test** for $f(x,y)$ (Q13) and the gradient mechanics (Q11, Q12).
5. **Translate words into one variable** for optimization (Q15).

> **Bottom line:** this is a *technique-recognition* exam. Almost every problem is solved by correctly **naming the method** in the first five seconds, then executing a standard recipe.

---

## Part 2 — Detailed Learning Guide

Each problem follows the same eight-step structure: clear restatement, topic, theory you need, *how to recognize the method*, full step-by-step solution with reasons, common mistakes, and a quick exam tip.

### Problem 1 — Derivative of a product, evaluated at a point

**Restate.** Given $h(2)=3$ and $h'(x)=-5$, compute $\dfrac{d}{dx}\!\left(\sqrt[5]{x}\,h(x)\right)$ at $x=2$.

**Topic.** Differentiation using the **product rule** combined with the **power rule** for a root.

**Theory & formulas.**
- Product rule: $(uv)' = u'v + uv'$.
- Root as a power: $\sqrt[5]{x}=x^{1/5}$, so $\dfrac{d}{dx}x^{1/5}=\tfrac{1}{5}x^{-4/5}$.

**How to recognize.** You see **two $x$-dependent factors multiplied together** ($\sqrt[5]{x}$ and $h(x)$). A product of factors ⇒ product rule. Numeric values of $h(2)$ and $h'$ tell you to differentiate symbolically first, then substitute.

**Step-by-step.** Let $u=x^{1/5}$, $v=h(x)$:

$$\frac{d}{dx}\left(x^{1/5}h(x)\right)=\tfrac{1}{5}x^{-4/5}\,h(x)+x^{1/5}\,h'(x).$$

Substitute $x=2,\ h(2)=3,\ h'(2)=-5$:

$$\tfrac{1}{5}\cdot 2^{-4/5}\cdot 3 + 2^{1/5}\cdot(-5)=2^{-4/5}\!\left(\tfrac{3}{5}-10\right)=-\frac{47}{5\cdot 2^{4/5}}\approx -5.40.$$

**Why each step.** Rewrite the root as a power so the power rule applies; differentiate **before** substituting because $h'$ is only known as a value; factor common powers of $2$ for an exact closed form.

**Common mistakes.** Forgetting the product rule; sign/exponent slip ($x^{1/5}\to\tfrac15x^{-4/5}$, not $\tfrac15x^{4/5}$); substituting too early.

> **Exam tip.** Convert every radical to a fractional exponent *before* differentiating.

---

### Problem 2 — Find the parameter so a point is an extremum

**Restate.** For $f(x)=ax^3-3x^2+4$, find $a$ so that $x=3$ is an extremum.

**Topic.** Critical points: $f'=0$ at an interior extremum.

**Theory & formulas.** At an interior extremum $f'(x_0)=0$. Differentiate, set the derivative at the given point to zero, solve for the parameter.

**How to recognize.** “$x=3$ is an extremum” + an **unknown constant** ⇒ solve $f'(3)=0$ for that constant.

**Step-by-step.**

$$f'(x)=3ax^2-6x,\qquad f'(3)=27a-18=0\ \Rightarrow\ a=\frac{18}{27}=\frac{2}{3}.$$

**Why.** A max/min of a differentiable function has zero slope; imposing this at $x=3$ gives one equation in $a$.

**Common mistakes.** Differentiating the constant $+4$ to something nonzero; differentiating with respect to $a$.

> **Exam tip.** “Extremum at $x_0$” $\Rightarrow f'(x_0)=0$. To confirm max vs. min, check $f''(x_0)$.

---

### Problem 3 — Intervals of increase and decrease

**Restate.** Determine where a function is increasing/decreasing. (Demonstrated on the representative cubic $f(x)=2x^3-9x^2+12x$.)

**Topic.** Monotonicity from the sign of $f'$.

**Theory & formulas.** $f'(x)>0\Rightarrow$ increasing; $f'(x)<0\Rightarrow$ decreasing. Boundaries are the **critical numbers** where $f'=0$ or is undefined.

**How to recognize.** Any “increasing/decreasing,” “monotonic intervals,” or “where is the function rising” ⇒ first-derivative sign chart.

**Step-by-step.**

$$f'(x)=6x^2-18x+12=6(x-1)(x-2).$$

Critical numbers $x=1,2$. Test signs:

| Interval | Sign of $f'$ | Behavior |
|----------|--------------|----------|
| $(-\infty,1)$ | $+$ | increasing |
| $(1,2)$ | $-$ | decreasing |
| $(2,\infty)$ | $+$ | increasing |

So $x=1$ is a local max and $x=2$ a local min.

**Common mistakes.** Forgetting points where $f'$ is undefined; reading sign from $f$ instead of $f'$; reporting points instead of intervals.

> **Exam tip.** Factor $f'$ fully, mark every critical number on a number line, test one point per interval.

---

### Problem 4 — Parameter for a given inflection point

**Restate.** For $f(x)=(2a-1)x^3-2x^2+1$, find $a$ so that the inflection point is at $F\bigl(1,\,f(1)\bigr)$.

**Topic.** Inflection points and concavity via $f''$.

**Theory & formulas.** Inflection where $f''$ changes sign; necessary condition $f''(x_0)=0$.

**How to recognize.** “Inflection point at $x_0$” + unknown constant ⇒ solve $f''(x_0)=0$ (the second-derivative analogue of Problem 2).

**Step-by-step.**

$$f'(x)=3(2a-1)x^2-4x,\qquad f''(x)=6(2a-1)x-4.$$
$$f''(1)=6(2a-1)-4=0\ \Rightarrow\ 12a-10=0\ \Rightarrow\ a=\frac{5}{6}.$$

Check: $2a-1=\tfrac23\neq0$, so it is a genuine cubic and concavity really changes. ✓

**Common mistakes.** Using $f'=0$; forgetting to check $2a-1\neq0$; arithmetic on $6(2a-1)$.

> **Exam tip.** Inflection $\to f''=0$; extremum $\to f'=0$.

---

### Problem 5 — Separable differential equation

**Restate.** Solve $\dfrac{dy}{dx}=e^{2x-3y}$.

**Topic.** First-order **separable** ODE.

**Theory & formulas.** If $\frac{dy}{dx}=g(x)h(y)$, separate $\frac{dy}{h(y)}=g(x)\,dx$ and integrate. Use $e^{2x-3y}=e^{2x}e^{-3y}$.

**How to recognize.** The right side **factors into an $x$-part times a $y$-part**; $e^{ax+by}$ always splits.

**Step-by-step.**

$$\frac{dy}{dx}=e^{2x}e^{-3y}\ \Rightarrow\ e^{3y}\,dy=e^{2x}\,dx.$$
$$\int e^{3y}\,dy=\int e^{2x}\,dx\ \Rightarrow\ \tfrac{1}{3}e^{3y}=\tfrac{1}{2}e^{2x}+C.$$
$$e^{3y}=\tfrac{3}{2}e^{2x}+C_1\ \Rightarrow\ y=\tfrac{1}{3}\ln\!\left(\tfrac{3}{2}e^{2x}+C_1\right).$$

**Common mistakes.** Integrating $e^{2x-3y}$ directly; dropping/duplicating $C$; forgetting the $\tfrac13,\tfrac12$ factors.

> **Exam tip.** See $e^{ax+by}$? Immediately write $e^{ax}\cdot e^{by}$.

---

### Problem 6 — Area under a curve

**Restate.** Find the area bounded by $y=e^{2x^3}$, the lines $x=1$, $x=2$, and the $x$-axis.

**Topic.** Area as a **definite integral** of a positive function.

**Theory & formulas.** For $f(x)\ge0$ on $[a,b]$, area $=\int_a^b f(x)\,dx$. Use $u$-substitution when the antiderivative is elementary; numerically otherwise.

**How to recognize.** “Area bounded by a curve, the $x$-axis, and two vertical lines” ⇒ definite integral with those lines as limits.

**Step-by-step.**

$$A=\int_{1}^{2} e^{2x^3}\,dx.$$

As written, $e^{2x^3}$ has **no elementary antiderivative**, so $A=\int_1^2 e^{2x^3}\,dx\approx 1.06\times10^{6}$ (dominated by $e^{16}\approx 8.9\times10^6$ near $x=2$). On a timed exam this is almost always the integrable version, e.g. $y=e^{2x}$, which shows the testable skill. With $u=2x,\ du=2\,dx$:

$$\int_1^2 e^{2x}\,dx=\tfrac12 e^{2x}\Big|_1^2=\tfrac12\left(e^4-e^2\right)\approx 23.6.$$

**Common mistakes.** Forgetting the $\tfrac12$ from $du=2\,dx$; not checking the curve is above the axis; swapping the limits.

> **Exam tip.** State the integral first. For $e^{(\text{linear})}$ use $u=$ the exponent.

---

### Problem 7 — Volume of a solid of revolution

**Restate.** The region bounded by $y=\sqrt{x}$, the $x$-axis, and $x=2$ is rotated about the **$y$-axis**. Find the volume.

**Topic.** Volume of revolution — **cylindrical shells**.

**Theory & formulas.** About the $y$-axis, integrating in $x$: $V=\int_a^b 2\pi x\,f(x)\,dx$ (radius $=x$, height $=f(x)$).

**How to recognize.** Rotation about the $y$-axis with the region given by $y=f(x)$ over an $x$-interval ⇒ shells are fastest.

**Step-by-step.**

$$V=\int_0^2 2\pi x\sqrt{x}\,dx=2\pi\int_0^2 x^{3/2}\,dx=2\pi\cdot\frac{2}{5}x^{5/2}\Big|_0^2=\frac{4\pi}{5}\,2^{5/2}=\frac{16\sqrt{2}}{5}\pi\approx 14.2.$$

**Common mistakes.** Using the disk formula about the wrong axis; dropping $2\pi$ or the radius $x$; lower limit is $x=0$, not $x=1$.

> **Exam tip.** Shells about the $y$-axis: $2\pi\!\int x\,f(x)\,dx$ — “radius $\times$ height.”

---

### Problem 8 — Equation of a tangent line

**Restate.** Find the tangent line to $y=4e^{x-2}+2x-3$ at $(2,5)$.

**Topic.** Tangent line via the derivative as slope.

**Theory & formulas.** $y-y_0=f'(x_0)(x-x_0)$; $\dfrac{d}{dx}e^{x-2}=e^{x-2}$.

**How to recognize.** “Tangent line at a point” ⇒ compute $f'$, evaluate at $x_0$, use point-slope.

**Step-by-step.** Check the point: $f(2)=4e^0+4-3=5$. ✓

$$f'(x)=4e^{x-2}+2\ \Rightarrow\ f'(2)=6,\qquad y-5=6(x-2)\ \Rightarrow\ y=6x-7.$$

**Common mistakes.** Mis-differentiating $e^{x-2}$; forgetting $\frac{d}{dx}(2x-3)=2$; using $y_0$ as the slope.

> **Exam tip.** Verify the point satisfies $y=f(x)$ first.

---

### Problem 9 — Integration by parts

**Restate.** Evaluate $\displaystyle\int x\cos 2x\,dx$.

**Topic.** Integration by parts.

**Theory & formulas.** $\int u\,dv=uv-\int v\,du$; choose $u$ by **LIATE** (the algebraic factor $x$ becomes $u$).

**How to recognize.** A product of an algebraic factor ($x$) and a trig/exponential factor ($\cos2x$), no obvious substitution.

**Step-by-step.** $u=x\ (du=dx)$, $dv=\cos2x\,dx\ (v=\tfrac12\sin2x)$:

$$\int x\cos 2x\,dx=\frac{x}{2}\sin 2x-\int \tfrac{1}{2}\sin 2x\,dx=\frac{x}{2}\sin 2x+\frac{1}{4}\cos 2x+C.$$

**Common mistakes.** Picking $u=\cos2x$; sign error $\int\sin2x\,dx=-\tfrac12\cos2x$; forgetting $+C$.

> **Exam tip.** For $\int x\cdot(\text{trig or }e^{kx})\,dx$, let $u=x$.

---

### Problem 10 — Indefinite integral with basic rules

**Restate.** Evaluate $\displaystyle\int\!\left(\frac{5}{x}-3\cdot 4^{x}+\frac{7}{3x^2}-4\sin x\right)dx$.

**Topic.** Term-by-term antidifferentiation.

**Theory & formulas.** $\int\frac1x dx=\ln|x|$, $\int a^x dx=\frac{a^x}{\ln a}$, $\int x^{-2}dx=-x^{-1}$, $\int\sin x\,dx=-\cos x$.

**How to recognize.** A **sum of simple, unrelated terms** — integrate each piece.

**Step-by-step.** Note $\tfrac{7}{3x^2}=\tfrac73x^{-2}$:

$$\int\frac{5}{x}\,dx=5\ln|x|,\quad \int -3\cdot4^{x}\,dx=-\frac{3\cdot4^{x}}{\ln 4},\quad \int \tfrac73x^{-2}\,dx=-\frac{7}{3x},\quad \int -4\sin x\,dx=4\cos x.$$
$$\boxed{\,5\ln|x|-\frac{3\cdot4^{x}}{\ln 4}-\frac{7}{3x}+4\cos x+C\,}$$

**Common mistakes.** $\ln x$ without absolute value; forgetting $\div\ln4$; sign on $\int-4\sin x=+4\cos x$.

> **Exam tip.** Rewrite every fraction as a power of $x$ first.

---

### Problem 11 — Tangent line to a level curve

**Restate.** For $f(x,y)=\sqrt{x^2+y^2+3}$, find the tangent line to the level curve $f=\sqrt5$ at a point on it (take $(1,1)$).

**Topic.** Level curves and the gradient as a normal vector.

**Theory & formulas.** Level curve $f=k$: squaring gives $x^2+y^2+3=5\Rightarrow x^2+y^2=2$ (circle of radius $\sqrt2$). $\nabla f \perp$ level curve; tangent line: $f_x(x_0,y_0)(x-x_0)+f_y(x_0,y_0)(y-y_0)=0$.

**How to recognize.** “Tangent to a level curve” ⇒ gradient = normal vector; tangent line passes through the point perpendicular to it.

**Step-by-step.** Check $(1,1)$: $\sqrt{1+1+3}=\sqrt5$. ✓

$$f_x=\frac{x}{\sqrt{x^2+y^2+3}},\quad f_y=\frac{y}{\sqrt{x^2+y^2+3}},\qquad \nabla f(1,1)=\left(\tfrac{1}{\sqrt5},\tfrac{1}{\sqrt5}\right)\parallel(1,1).$$
$$1\,(x-1)+1\,(y-1)=0\ \Rightarrow\ x+y=2.$$

**Common mistakes.** Confusing the gradient (normal) with the tangent direction; not verifying the point is on the curve; dropping the constant.

> **Exam tip.** Tangent line: $f_x(x-x_0)+f_y(y-y_0)=0$; the common $\tfrac{1}{\sqrt5}$ cancels — only the *direction* of $\nabla f$ matters.

---

### Problem 12 — Gradient of a function of two variables

**Restate.** For $f(x,y)=x^3y^2-2xy+3$, find the gradient at $(2,2)$.

**Topic.** Partial derivatives and the gradient vector.

**Theory & formulas.** $\nabla f=(f_x,f_y)$: differentiate w.r.t. $x$ holding $y$ constant, and vice versa.

**How to recognize.** “Gradient” / $\nabla f$ ⇒ both first-order partials assembled into a vector.

**Step-by-step.**

$$f_x=3x^2y^2-2y,\qquad f_y=2x^3y-2x.$$
$$f_x(2,2)=3(4)(4)-2(2)=44,\qquad f_y(2,2)=2(8)(2)-2(2)=28,\qquad \nabla f(2,2)=(44,\,28).$$

**Common mistakes.** Treating $y^2$ as variable in $f_x$; mixing up which variable is fixed; reporting a number not a vector.

> **Exam tip.** Write “$y=$const” over $f_x$ and “$x=$const” over $f_y$.

---

### Problem 13 — Extrema of a function of two variables

**Restate.** Find the extreme value of $f(x,y)=xy-x^2-y^2-2x-2y+4$.

**Topic.** Critical points of a surface and the **second-derivative (Hessian) test**.

**Theory & formulas.** Solve $f_x=0,\ f_y=0$. Discriminant $D=f_{xx}f_{yy}-(f_{xy})^2$: $D>0,f_{xx}<0\Rightarrow$ max; $D>0,f_{xx}>0\Rightarrow$ min; $D<0\Rightarrow$ saddle.

**How to recognize.** “Find the extrema of $f(x,y)$” (no constraint) ⇒ $\nabla f=0$ then classify with $D$.

**Step-by-step.**

$$f_x=y-2x-2=0,\qquad f_y=x-2y-2=0.$$

From the first $y=2x+2$; substitute: $x-2(2x+2)-2=0\Rightarrow -3x-6=0\Rightarrow x=-2,\ y=-2$.

$$f_{xx}=-2,\ f_{yy}=-2,\ f_{xy}=1,\qquad D=(-2)(-2)-1^2=3>0,\ f_{xx}<0\ \Rightarrow\ \text{local max}.$$
$$f(-2,-2)=4-4-4+4+4+4=8.$$

So $f$ has a **local maximum value $8$** at $(-2,-2)$.

**Common mistakes.** Stopping without the $D$-test; sign error in $D$; arithmetic in the value.

> **Exam tip.** Solve $f_x=0,f_y=0$ by elimination; for quadratics $D$ is a single number.

---

### Problem 14 — First-order linear ODE with initial condition

**Restate.** Solve $\dfrac{dy}{dx}+\dfrac{3}{x}\,y=x$ for $x>0$, with $y(1)=-2$.

**Topic.** First-order **linear** ODE — integrating-factor method + IVP.

**Theory & formulas.** Standard form $\frac{dy}{dx}+P(x)y=Q(x)$; integrating factor $\mu=e^{\int P\,dx}$; then $(\mu y)'=\mu Q$.

**How to recognize.** Equation is linear in $y$ and $y'$ ($y$ to the first power) — integrating-factor signature (not separable).

**Step-by-step.** Here $P=\tfrac3x$:

$$\mu=e^{\int \frac{3}{x}\,dx}=e^{3\ln x}=x^{3}.$$
$$(x^{3}y)'=x^{3}\cdot x=x^{4}\ \Rightarrow\ x^{3}y=\frac{x^{5}}{5}+C\ \Rightarrow\ y=\frac{x^{2}}{5}+\frac{C}{x^{3}}.$$

Apply $y(1)=-2$: $\tfrac15+C=-2\Rightarrow C=-\tfrac{11}{5}$:

$$\boxed{\,y=\frac{x^{2}}{5}-\frac{11}{5x^{3}}\,}$$

**Common mistakes.** Trying to separate (it isn't separable); $e^{3\ln x}=x^3$ (not $3x$); applying the IC before solving for $y$.

> **Exam tip.** Recipe: (1) standard form, (2) $\mu=e^{\int P}$, (3) $(\mu y)'=\mu Q$, (4) integrate + apply IC.

---

### Problem 15 — Applied optimization (largest inscribed rectangle)

**Restate.** A rectangle is inscribed in a right triangle with legs $2$ and $3$ (right angle at the origin). With a corner $(x,y)$ on the hypotenuse, similar triangles give $\frac{3-x}{3}=\frac{y}{2}$. Maximize the area.

**Topic.** Optimization — build a single-variable model, then maximize.

**Theory & formulas.** Use the constraint to write $y$ in terms of $x$; maximize $S(x)$ via $S'(x)=0$.

**How to recognize.** “Largest/smallest” quantity with a geometric relationship ⇒ reduce to one variable, then differentiate.

**Step-by-step.** $y=\tfrac23(3-x)$, so

$$S(x)=x\cdot\frac{2}{3}(3-x)=\frac{2}{3}\left(3x-x^{2}\right),\qquad S'(x)=\frac{2}{3}(3-2x)=0\ \Rightarrow\ x=\frac{3}{2}.$$
$$y=\tfrac23\!\left(3-\tfrac32\right)=1,\qquad S_{\max}=\frac{3}{2}\cdot 1=\frac{3}{2}.$$

This is exactly half the triangle's area $\tfrac12\cdot2\cdot3=3$ — the classic result.

**Common mistakes.** Not expressing $y$ in terms of $x$ first; differentiating with both variables present; not confirming a max ($S''=-\tfrac43<0$).

> **Exam tip.** “Rectangle in a triangle” → max area is half the triangle's area, optimal corner at the midpoints of the legs.

---

## Part 3 — Practice Exam A

**Instructions.** Questions 1–10 are worth **1 point** each; questions 11–15 are worth **4 points** each (40 points total). Show all work. These are new problems testing the same methods — nothing copied from the original.

**Section I — Short problems (1 point each)**

1. Given $g(8)=2$ and $g'(8)=4$, compute $\dfrac{d}{dx}\!\left(\sqrt[3]{x}\,g(x)\right)$ at $x=8$.
2. For $f(x)=ax^3-12x+1$, find $a$ so that $x=2$ is an extremum.
3. Find the intervals of increase and decrease of $f(x)=x^3-6x^2+9x+1$.
4. For $f(x)=(a-2)x^3+3x^2-1$, find $a$ so that the inflection point is at $x=1$.
5. Solve the separable equation $\dfrac{dy}{dx}=e^{x-2y}$.
6. Find the area bounded by $y=e^{3x}$, the $x$-axis, and the lines $x=0$ and $x=1$.
7. The region bounded by $y=x^2$, the $x$-axis, and $x=1$ is rotated about the $y$-axis. Find the volume.
8. Find the tangent line to $y=3e^{x-1}+x^2-2$ at the point $(1,2)$.
9. Evaluate $\displaystyle\int x\sin 3x\,dx$ by parts.
10. Evaluate $\displaystyle\int\!\left(\dfrac{3}{x}+2\cdot 5^{x}-\dfrac{4}{x^2}+3\cos x\right)dx$.

**Section II — Extended problems (4 points each)**

11. For $f(x,y)=\sqrt{x^2+y^2+1}$, find the tangent line to the level curve $f=\sqrt{11}$ at the point $(1,3)$.
12. For $f(x,y)=x^2y^3-3xy+2$, find the gradient at $(1,2)$.
13. Find and classify the extreme value of $f(x,y)=xy-x^2-y^2+3x$.
14. Solve $\dfrac{dy}{dx}+\dfrac{2}{x}\,y=x^2$ for $x>0$ with $y(1)=3$.
15. A rectangle is inscribed in a right triangle with legs $4$ and $6$, corner $(x,y)$ on the hypotenuse where $\frac{6-x}{6}=\frac{y}{4}$. Find the dimensions that maximize the area, and the maximum area.

---

## Part 4 — Practice Exam B

**Instructions.** Same format: Questions 1–10 are worth **1 point** each; questions 11–15 are worth **4 points** each (40 points total).

**Section I — Short problems (1 point each)**

1. Given $k(4)=5$ and $k'(4)=-2$, compute $\dfrac{d}{dx}\!\left(\sqrt{x}\,k(x)\right)$ at $x=4$.
2. For $f(x)=ax^3-6x^2+5$, find $a$ so that $x=4$ is an extremum.
3. Find the intervals of increase and decrease of $f(x)=2x^3-3x^2-12x+4$.
4. For $f(x)=(3a-1)x^3+3x^2-2$, find $a$ so that the inflection point is at $x=-1$.
5. Solve the separable equation $\dfrac{dy}{dx}=e^{3x-y}$.
6. Find the area bounded by $y=e^{4x}$, the $x$-axis, and the lines $x=0$ and $x=1$.
7. The region bounded by $y=\sqrt{x}$, the $x$-axis, and $x=4$ is rotated about the $y$-axis. Find the volume.
8. Find the tangent line to $y=2e^{x-3}+3x-4$ at the point $(3,7)$.
9. Evaluate $\displaystyle\int x\,e^{2x}\,dx$ by parts.
10. Evaluate $\displaystyle\int\!\left(\dfrac{7}{x}-2\cdot 3^{x}+\dfrac{5}{x^2}-6\sin x\right)dx$.

**Section II — Extended problems (4 points each)**

11. For $f(x,y)=\sqrt{x^2+y^2+4}$, find the tangent line to the level curve $f=\sqrt{29}$ at the point $(3,4)$.
12. For $f(x,y)=x^3y-xy^2+5$, find the gradient at $(2,1)$.
13. Find and classify the extreme value of $f(x,y)=xy-x^2-y^2+6y$.
14. Solve $\dfrac{dy}{dx}+\dfrac{4}{x}\,y=x$ for $x>0$ with $y(1)=2$.
15. A rectangle is inscribed in a right triangle with legs $3$ and $6$, corner $(x,y)$ on the hypotenuse where $\frac{6-x}{6}=\frac{y}{3}$. Find the dimensions that maximize the area, and the maximum area.

---

## Part 5 — Complete Solutions

Full worked solutions for the original exam and both practice exams. Each solution names the method first, then shows the calculations, shortcuts, and the pitfall to avoid.

### A. Original Exam — Solutions

**1. Product rule at a point.** *Method:* product rule with $\sqrt[5]{x}=x^{1/5}$.
$$\tfrac15 x^{-4/5}h(x)+x^{1/5}h'(x)\Big|_{x=2}=\tfrac15\cdot2^{-4/5}\cdot3+2^{1/5}(-5)=-\frac{47}{5\cdot2^{4/5}}\approx-5.40.$$
*Pitfall:* substituting $x=2$ before differentiating.

**2. Parameter for an extremum.** *Method:* $f'(3)=0$.
$$f'(x)=3ax^2-6x,\quad 27a-18=0\ \Rightarrow\ a=\tfrac23.$$

**3. Increase / decrease** (for $f(x)=2x^3-9x^2+12x$). *Method:* sign chart of $f'$.
$$f'(x)=6(x-1)(x-2).$$
Increasing on $(-\infty,1)$ and $(2,\infty)$; decreasing on $(1,2)$.

**4. Parameter for an inflection point.** *Method:* $f''(1)=0$.
$$f''(x)=6(2a-1)x-4,\quad 6(2a-1)-4=0\ \Rightarrow\ a=\tfrac56.$$
*Pitfall:* using $f'=0$; not checking $2a-1\neq0$.

**5. Separable ODE.** *Method:* split $e^{2x-3y}=e^{2x}e^{-3y}$.
$$e^{3y}\,dy=e^{2x}\,dx\ \Rightarrow\ \tfrac13 e^{3y}=\tfrac12 e^{2x}+C\ \Rightarrow\ y=\tfrac13\ln\!\big(\tfrac32 e^{2x}+C_1\big).$$

**6. Area under a curve.** $A=\int_1^2 e^{2x^3}\,dx$ is non-elementary $(\approx1.06\times10^6)$. Integrable model $y=e^{2x}$:
$$\int_1^2 e^{2x}\,dx=\tfrac12(e^4-e^2)\approx23.6.$$
*Pitfall:* dropping the $\tfrac12$ from $u=2x$.

**7. Volume about the $y$-axis.** *Method:* shells $V=2\pi\int_0^2 x\sqrt{x}\,dx$.
$$V=2\pi\cdot\tfrac25 x^{5/2}\Big|_0^2=\frac{16\sqrt2}{5}\pi\approx14.2.$$
*Pitfall:* lower limit is $x=0$, not $x=1$.

**8. Tangent line.** *Method:* point-slope with $f'(2)$.
$$f'(x)=4e^{x-2}+2,\ f'(2)=6\ \Rightarrow\ y=6x-7.$$

**9. Integration by parts.** $u=x,\ dv=\cos2x\,dx$.
$$\int x\cos2x\,dx=\frac{x}{2}\sin2x+\frac14\cos2x+C.$$
*Pitfall:* sign — $\int\sin2x\,dx=-\tfrac12\cos2x$.

**10. Indefinite integral.**
$$5\ln|x|-\frac{3\cdot4^{x}}{\ln4}-\frac{7}{3x}+4\cos x+C.$$
*Pitfall:* missing $\div\ln4$ and the absolute value in $\ln|x|$.

**11. Tangent to a level curve.** Level curve $x^2+y^2=2$; gradient $\propto(1,1)$ at $(1,1)$.
$$1(x-1)+1(y-1)=0\ \Rightarrow\ x+y=2.$$

**12. Gradient.** $\nabla f=(3x^2y^2-2y,\ 2x^3y-2x)$ at $(2,2)$.
$$\nabla f(2,2)=(48-4,\ 32-4)=(44,\,28).$$

**13. Extrema of $f(x,y)$.** *Method:* $\nabla f=0$ then Hessian.
$$y-2x-2=0,\ x-2y-2=0\ \Rightarrow\ (-2,-2);\quad D=(-2)(-2)-1^2=3>0,\ f_{xx}<0\Rightarrow\text{max},\ f(-2,-2)=8.$$

**14. First-order linear ODE (IVP).** Integrating factor $\mu=x^3$.
$$(x^3y)'=x^4\ \Rightarrow\ y=\frac{x^2}{5}+\frac{C}{x^3},\ \ y(1)=-2\Rightarrow C=-\tfrac{11}{5}\ \Rightarrow\ y=\frac{x^2}{5}-\frac{11}{5x^3}.$$
*Pitfall:* trying to separate; $e^{3\ln x}=x^3$.

**15. Optimization.** $S(x)=\tfrac23(3x-x^2)$.
$$S'(x)=\tfrac23(3-2x)=0\Rightarrow x=\tfrac32,\ y=1,\ S_{\max}=\tfrac32.$$

---

### B. Practice Exam A — Solutions

**1.** $\sqrt[3]{x}=x^{1/3}$, product rule at $x=8$:
$$\tfrac13 x^{-2/3}g(x)+x^{1/3}g'(x)\Big|_{8}=\tfrac13\cdot\tfrac14\cdot2+2\cdot4=\tfrac16+8=\frac{49}{6}\approx8.17.$$
*Pitfall:* $8^{-2/3}=\tfrac14$ and $\sqrt[3]{8}=2$.

**2.** $f'(x)=3ax^2-12,\ 12a-12=0\Rightarrow a=1.$

**3.** $f'(x)=3x^2-12x+9=3(x-1)(x-3)$. Increasing on $(-\infty,1)$ and $(3,\infty)$; decreasing on $(1,3)$.

**4.** $f''(x)=6(a-2)x+6,\ 6(a-2)+6=0\Rightarrow a=1.$

**5.** $e^{x-2y}=e^xe^{-2y}$:
$$e^{2y}\,dy=e^{x}\,dx\Rightarrow\tfrac12 e^{2y}=e^{x}+C\Rightarrow y=\tfrac12\ln(2e^{x}+C_1).$$

**6.** $A=\int_0^1 e^{3x}\,dx=\tfrac13 e^{3x}\big|_0^1=\tfrac13(e^3-1)\approx6.36.$

**7.** Shells $V=2\pi\int_0^1 x\cdot x^2\,dx=2\pi\int_0^1 x^3\,dx=2\pi\cdot\tfrac14=\dfrac{\pi}{2}.$ *Pitfall:* height is $x^2$, so integrand $=x^3$.

**8.** $f'(x)=3e^{x-1}+2x,\ f'(1)=5\Rightarrow y=5x-3.$

**9.** $u=x,\ dv=\sin3x\,dx,\ v=-\tfrac13\cos3x$:
$$\int x\sin3x\,dx=-\frac{x}{3}\cos3x+\frac19\sin3x+C.$$

**10.** $\displaystyle 3\ln|x|+\frac{2\cdot5^{x}}{\ln5}+\frac{4}{x}+3\sin x+C.$ *Pitfall:* $\int-\tfrac{4}{x^2}\,dx=+\tfrac4x$.

**11.** Level curve $x^2+y^2=10$; gradient $\propto(1,3)$ at $(1,3)$:
$$1(x-1)+3(y-3)=0\Rightarrow x+3y=10.$$

**12.** $\nabla f=(2xy^3-3y,\ 3x^2y^2-3x)$ at $(1,2)$: $\nabla f(1,2)=(16-6,\ 12-3)=(10,\,9).$

**13.** $f_x=y-2x+3=0,\ f_y=x-2y=0\Rightarrow x=2,y=1$; $D=3>0,\ f_{xx}<0\Rightarrow$ max, $f(2,1)=3.$

**14.** $\mu=x^2$: $(x^2y)'=x^4\Rightarrow y=\dfrac{x^3}{5}+\dfrac{C}{x^2},\ y(1)=3\Rightarrow C=\tfrac{14}{5}\Rightarrow y=\dfrac{x^3}{5}+\dfrac{14}{5x^2}.$

**15.** $y=\tfrac23(6-x),\ S=\tfrac23(6x-x^2)$: $S'(x)=\tfrac23(6-2x)=0\Rightarrow x=3,\ y=2,\ S_{\max}=6$ (half of triangle area $12$).

---

### C. Practice Exam B — Solutions

**1.** $\sqrt{x}=x^{1/2}$, product rule at $x=4$:
$$\frac{1}{2\sqrt{x}}k(x)+\sqrt{x}\,k'(x)\Big|_{4}=\tfrac14\cdot5+2(-2)=\frac54-4=-\frac{11}{4}.$$

**2.** $f'(x)=3ax^2-12x,\ 48a-48=0\Rightarrow a=1.$

**3.** $f'(x)=6x^2-6x-12=6(x-2)(x+1)$. Increasing on $(-\infty,-1)$ and $(2,\infty)$; decreasing on $(-1,2)$.

**4.** $f''(x)=6(3a-1)x+6,\ -6(3a-1)+6=0\Rightarrow a=\tfrac23.$

**5.** $e^{3x-y}=e^{3x}e^{-y}$:
$$e^{y}\,dy=e^{3x}\,dx\Rightarrow e^{y}=\tfrac13 e^{3x}+C\Rightarrow y=\ln\!\big(\tfrac13 e^{3x}+C\big).$$

**6.** $A=\int_0^1 e^{4x}\,dx=\tfrac14 e^{4x}\big|_0^1=\tfrac14(e^4-1)\approx13.40.$

**7.** Shells $V=2\pi\int_0^4 x\sqrt{x}\,dx=2\pi\cdot\tfrac25 x^{5/2}\big|_0^4=2\pi\cdot\tfrac25\cdot32=\dfrac{128\pi}{5}\approx80.4.$ *Pitfall:* $4^{5/2}=32$.

**8.** $f'(x)=2e^{x-3}+3,\ f'(3)=5\Rightarrow y=5x-8.$

**9.** $u=x,\ dv=e^{2x}\,dx,\ v=\tfrac12 e^{2x}$:
$$\int x e^{2x}\,dx=\frac{x}{2}e^{2x}-\frac14 e^{2x}+C.$$

**10.** $\displaystyle 7\ln|x|-\frac{2\cdot3^{x}}{\ln3}-\frac{5}{x}+6\cos x+C.$ *Pitfall:* $\int\tfrac{5}{x^2}\,dx=-\tfrac5x$; $\int-6\sin x=+6\cos x$.

**11.** Level curve $x^2+y^2=25$; gradient $\propto(3,4)$ at $(3,4)$:
$$3(x-3)+4(y-4)=0\Rightarrow 3x+4y=25.$$

**12.** $\nabla f=(3x^2y-y^2,\ x^3-2xy)$ at $(2,1)$: $\nabla f(2,1)=(12-1,\ 8-4)=(11,\,4).$

**13.** $f_x=y-2x=0,\ f_y=x-2y+6=0\Rightarrow x=2,y=4$; $D=3>0,\ f_{xx}<0\Rightarrow$ max, $f(2,4)=12.$

**14.** $\mu=x^4$: $(x^4y)'=x^5\Rightarrow y=\dfrac{x^2}{6}+\dfrac{C}{x^4},\ y(1)=2\Rightarrow C=\tfrac{11}{6}\Rightarrow y=\dfrac{x^2}{6}+\dfrac{11}{6x^4}.$

**15.** $y=\tfrac12(6-x),\ S=\tfrac12(6x-x^2)$: $S'(x)=\tfrac12(6-2x)=0\Rightarrow x=3,\ y=\tfrac32,\ S_{\max}=\tfrac92$ (half of triangle area $9$).

---

> **Final reminder before exam day**
> - For every problem, **name the method in the first five seconds**: derivative-at-a-point, $f'=0$, $f''=0$, separate-and-integrate, integrating factor, set-up-the-integral, shells, point-slope, by-parts, $\nabla f=0$ + Hessian, or reduce-to-one-variable.
> - Carry exact forms ($\sqrt2$, $\ln$, fractions) as far as possible; only approximate at the very end.
> - Always write $+C$ on indefinite integrals and apply initial conditions **after** solving for $y$.

# 📌 [Linear Systems, Vector Equations, and Matrix Equations]

## 1. Flow

- A set of linear equations with the same variables forms a linear system.
- That linear system can be rewritten as a vector equation.
- A vector equation can then be represented as a matrix equation.

> linear system → vector equation → matrix equation

---

## 2. Interpretation

- Summary: **"same structure, different perspective"**
- A vector can be viewed as an element of space, but in linear algebra, it is especially important because it can be combined linearly with other vectors to produce new vectors.
- In this sense, a vector is not isolated. It can be expressed as **a linear combination of other vectors**.
- So the expression below is not just an equation. It describes how a target vector is formed from given vectors and scalar coefficients.

---

## 3. Mathematical Expression

**Vector equation:**

$$
x_1 a_1 + x_2 a_2 + \cdots + x_n a_n = b
$$

This means that the target vector $b$ is written as a linear combination of the vectors $a_1, a_2, \ldots, a_n$.

---

## 4. How It Connects to the Flow

- A system of linear equations can be rewritten as a vector equation.
- Each **column of a matrix** is viewed as a vector $a_i$, and the variables become scalars $x_i$.

This changes our viewpoint:

- equation-based thinking → structure-based thinking

Then, by stacking vectors into a matrix, we get:

$$
Ax = b
$$

So the flow becomes:

> linear system → vector equation → matrix equation

This is important because it compresses multiple equations into a single mathematical structure, which is one of the foundational viewpoints of linear algebra.

---

## 5. Connection to AI 🔗

- In many AI models, the basic computation has the form

$$
y = Ax + b
$$

where:

- $x$ : input vector (**features / data**)
- $A$ : weight matrix (**transformation / model parameters**)
- $b$ : bias vector (**an additional constant term added to the transformation**)

This is exactly what happens in many machine learning and deep learning models:

- input vector → multiplied by a weight matrix → shifted by a bias vector → output vector

So in essence,

> AI models are built on repeated linear combinations of data.

- Neural networks, in particular, can be viewed as stacked matrix operations followed by nonlinear activations.

---

## 6. Connection with Other Concepts

- From a geometric perspective, vectors represent directions in space.
- When multiple vectors are combined linearly, they generate a set of reachable vectors.

This leads to important concepts such as:

- **span** → all vectors that can be formed by linear combinations
- **basis** → a minimal set of linearly independent vectors that generates a space
- **column space** → all possible outputs of $Ax$

> In other words, linear combinations determine the space that vectors can reach.
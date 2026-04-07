# 📌 [Linear Transformation]

## 1. Flow

- In the previous topic, we studied how vectors generate spaces through **span**, **basis**, and **column space**.
- There, a matrix was understood mainly through its columns and the space they generate.
- Now the focus shifts from the structure of generated spaces to the idea of a **transformation** itself.
- This leads naturally to **linear transformations**, which describe how vectors are mapped from one space to another while preserving linear structure.

> span / basis / column space → linear transformation

---

## 2. Interpretation

- Summary: **"a linear transformation is a mapping that sends vectors from one space to another while preserving linear structure"**
- A **linear transformation** is a function that maps vectors in an input space to vectors in an output space.
- In other words, it is a **mapping between spaces**:

$$
T : \mathbb{R}^n \to \mathbb{R}^m
$$

- This means that each input vector $x \in \mathbb{R}^n$ is assigned to an output vector $T(x) \in \mathbb{R}^m$.
- So a linear transformation is not only about individual vectors, but also about how an entire **space** is mapped into another space.
- What makes this mapping **linear** is that it preserves the two basic linear operations:

$$
T(u+v) = T(u) + T(v)
$$

$$
T(cu) = cT(u)
$$

- This means that the transformation preserves the way vectors combine.
- It does not move vectors arbitrarily; it maps them in a consistent way that keeps their linear relationships.
- Through this mapping, vectors can be **combined, emphasized, compressed, or projected** into a new space.

A **matrix transformation** is a concrete form of a linear transformation:

$$
T(x) = Ax
$$

- Here, the matrix $A$ gives the rule that determines how each input vector is mapped to an output vector.

---

## 3. Mathematical Expression

### (1) Matrix Transformation

$$
T(x) = Ax
$$

A matrix transformation maps a vector $x \in \mathbb{R}^n$ to an output vector in $\mathbb{R}^m$.

---

### (2) Linear Transformation Conditions

$$
T(u+v) = T(u) + T(v)
$$

Preserves vector addition.

$$
T(cu)=cT(u)
$$

Preserves scalar multiplication.

---

## 4. How It Connects to the Flow

A linear transformation is not just about individual vectors, but about a consistent **mapping rule** from an input space to an output space.  
Each input vector is mapped to an output vector, and because the transformation is linear, the way vectors combine is preserved under that mapping.

If a vector is written as a linear combination, then applying $T$ gives:

$$
T(x_1v_1 + x_2v_2 + \cdots + x_nv_n)
=
x_1T(v_1) + x_2T(v_2) + \cdots + x_nT(v_n)
$$

This means that once we know where the basic vectors are mapped, we can determine how every other vector is mapped as well.  
That is why linear transformations are closely connected to matrices: in a matrix transformation $T(x) = Ax$, the columns of $A$ tell us how the basis vectors are mapped.

From this viewpoint, a matrix becomes a concrete description of a mapping.  
And the column space tells us which outputs are actually reachable through that mapping.

So the key question becomes:

> where does the transformation send vectors, and how much of the output space can it reach?

---

## 5. Connection to AI 🔗

- In AI, many models can be understood as repeated mappings from one vector space to another.
- A matrix transformation is one of the basic ways a model maps data into a new representation.

This idea appears in several important AI applications:

- **linear layers** → mixing input features to produce new features
- **representation learning** → learning transformations that make useful patterns easier to represent
- **embedding projections** → mapping data into spaces where similarity and structure become clearer
- **dimensionality change** → expanding or compressing representations by changing the size of the space
- **feature extraction** → emphasizing important directions and reducing less useful ones

This is why a linear transformation is so important in AI.  
A model learns matrices that map raw input vectors into more useful spaces, where important structure becomes easier to capture and use.

---

## 6. Connection with Other Concepts

These ideas naturally lead to several important questions about transformations:

- **kernel** → which vectors are mapped to zero
- **range / image** → which outputs can actually be reached
- **one-to-one** → whether different inputs always remain different after transformation
- **onto** → whether the whole output space can be reached
- **standard matrix** → how a transformation is represented as a matrix

> In other words, after understanding what a linear transformation is, the next step is to study how to analyze its behavior more precisely.
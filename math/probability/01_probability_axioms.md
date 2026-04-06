# 📌 [Probability Axioms]

## 1. Flow

- Probability starts from the question: **how can we mathematically describe uncertainty?**
  - One natural idea is the long-run relative frequency of an event.
  - But because that idea has limitations, modern probability theory starts from an **axiomatic approach**.

> Question about uncertainty → relative frequency intuition → axiomatical approach

---

## 2. Interpretation

- A common intuition is:

$$
P(E) = \lim_{n \to \infty} \frac{n(E)}{n}
$$

where $n(E)$ is the number of times event $E$ occurs in $n$ trials.

- This is intuitive, but it has limitations:
  - the limit is not guaranteed in advance
  - probability needs a more stable mathematical foundation

- So modern probability does not define probability by frequency itself.
- Instead, it assigns a value $P(E)$ to each event and requires that these values satisfy a few basic axioms.

> Relative frequency gives intuition, but axioms give the foundation

---

## 3. Mathematical Expression

Let $S$ denote the set of all possible outcomes, and let $E \subseteq S$ be an event.

A probability function $P$ satisfies:

### Axiom 1
$$
0 \leq P(E) \leq 1
$$

### Axiom 2
$$
P(S) = 1
$$

### Axiom 3
If $E_1, E_2, E_3, \dots$ are pairwise disjoint, then

$$
P\left(\bigcup_{i=1}^{\infty} E_i\right)=\sum_{i=1}^{\infty} P(E_i)
$$

---

## 4. How It Connects to the Flow

- The axioms do not determine specific probability values; they provide the basic rules that every probability assignment must satisfy.
- The actual values depend on the assumptions or beliefs we make about the situation.

> Axioms give the rules, and assumptions determine the values

---

## 5. Connection to AI 🔗

- In AI, probability is used to model uncertainty in data, prediction, and inference.
- This means that the quality of a probabilistic model depends on how well its assumptions match the actual situation.
- If the assumptions are reasonable, probability becomes a useful framework for learning from data and updating predictions.

> AI learning can be viewed from a probabilistic perspective:  
> modeling uncertainty, making assumptions about data, and updating predictions from observations

---

## 6. Connection with Other Concepts

- These axioms are the foundation of all later concepts in probability.
- Once probability is defined, the next step is to ask:

> how does probability change when new information is given?

- This naturally leads to:
  - **conditional probability**
  - **independence**

These ideas will lead naturally to Bayes' theorem, random variables, and probability distributions.
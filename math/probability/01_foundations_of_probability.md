# 📌 [Foundations of Probability]

## 1. Flow

- Probability starts from the question: **how can we mathematically describe uncertainty?**
- There are several ways to interpret probability:
  - as symmetry in equally likely cases
  - as long-run relative frequency
  - as degree of belief under given information
- However, to study probability in a mathematically consistent way, modern probability theory adopts an **axiomatic approach**.

> uncertainty → interpretations of probability → axiomatic foundation

---

## 2. Interpretation

Probability can be understood in several different ways.

### (1) Classical view
- Probability is based on **equally likely outcomes**.
- Example: when rolling a fair die, the probability of getting 1 is

$$
P(\{1\}) = \frac{1}{6}
$$

- **Strength:** simple and intuitive when symmetry is clear  
- **Limitation:** not all real situations have equally likely outcomes

### (2) Frequentist view
- Probability is understood as a **long-run relative frequency**.
- Example: if a coin is tossed many times, the proportion of heads is expected to get closer to 0.5.
- A common expression is

$$
P(E) = \lim_{n \to \infty} \frac{n(E)}{n}
$$

where $n(E)$ is the number of times event $E$ occurs in $n$ trials.

- **Strength:** connects probability to repeated experiments and observable data  
- **Limitation:** the limit is not guaranteed in advance, and not every situation can be repeated infinitely many times

### (3) Belief view
- Probability is understood as a **degree of belief** given current information.
- The value of probability may depend on what is known or assumed.
- Example: if we know dark clouds are forming, we may assign a higher probability to rain than we would under a clear sky.

- **Strength:** useful when probability must reflect partial knowledge or uncertainty about unique situations  
- **Limitation:** probability can depend on assumptions, so different information may lead to different values

> Probability can be interpreted in multiple ways, but these interpretations do not by themselves provide the full mathematical foundation.

---

## 3. Mathematical Expression

In modern probability theory, probability is treated as a **set function**:

$$
P:\text{events} \to [0,1]
$$

That is, probability assigns a value between 0 and 1 to each event.

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

- These different interpretations help us understand what probability is trying to express.
- The classical view emphasizes symmetry, the frequentist view emphasizes repeated trials, and the belief view emphasizes uncertainty under information.
- But regardless of interpretation, probability theory needs a common mathematical structure.
- That is why modern probability is built on axioms:
  - interpretations give intuition about meaning
  - axioms give the formal rules probability must satisfy

> Interpretations explain the meaning of probability, while axioms provide the mathematical foundation that makes the theory consistent.

---

## 5. Connection to AI 🔗

- In AI, probability is used to model **uncertainty in data, predictions, and inference**.
- A common assumption is that **data is generated from some underlying probability distribution**.
- Under this view, learning is not only about fitting data, but also about describing uncertainty in a principled way.
- This is why the **belief view** is especially important in AI:
  - probability represents what is believed given current information
  - observations are used to update those beliefs
- A probabilistic model becomes useful when its assumptions about the data-generating process are reasonably consistent with reality.

> In AI, probability is used both to model how data may be generated and to express and update beliefs under uncertainty.

---

## 6. Connection with Other Concepts

- Once probability is defined, the next natural question is:

> how should belief change when new information is given?

- This leads naturally to:
  - **conditional probability**
  - **independence**

- In particular, the belief view becomes especially important here:
  - probability is updated when new evidence is observed
  - this idea develops naturally into **Bayes’ theorem**

- From there, probability connects to:
  - random variables
  - probability distributions
  - probabilistic inference

> If probability measures belief under current information, then conditional probability tells us how that belief should change when new information arrives
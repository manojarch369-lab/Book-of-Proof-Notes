# Book-of-Proof-Notes
My Notes while studying 'Book of Proof'


# Chapter 1 [[Sets]] | [[Book of Proof]] | [[Richard Hammack]]

> [!quote] [[book_of_proof.pdf#page=15&selection=5,0,8,26&color=note|book_of_proof, p.3]]
> > All of mathematics can be described with sets

> [!PDF|note] [[book_of_proof.pdf#page=15&selection=8,28,12,33&color=note|book_of_proof, p.3]]
> > This becomes more and more apparent the deeper into mathematics you go. It will be apparent in most of your upper level courses, and certainly in this course. The theory of sets is a language that is perfectly suited to describing and explaining all types of mathematical structures.


## 1.1 Introduction to Sets

### [[Set]] (in [[Book of Proof]] by [[Richard Hammack]]) 
is a collection of objects, written inside curly braces.  
Example: {2, 4, 6, 8}

Sets may be:

- **Finite**, like {1, 2, 3}
    
- **Infinite**, like the set of integers ℤ = {..., −2, −1, 0, 1, 2, ...}
    

> [!note] Sets are fundamental objects in mathematics and are used to define nearly all other mathematical structures.

---

### [[Element]] (in [[Book of Proof]] by [[Richard Hammack]])

An **element** is a member of a set.

Notation:

- `x ∈ A` means “x is in A”
    
- `x ∉ A` means “x is not in A”
    

Example:

- 2 ∈ {1, 2, 3}
    
- 5 ∉ {1, 2, 3}
    

> [!quote] “A set is a collection of things.” — _[[Richard Hammack]]_

> [!quote] “Think of a set as a box with things in it.” — _[[Richard Hammack]]_

---

### [[Empty Set]] (in [[Book of Proof]] by [[Richard Hammack]])

The **empty set** contains no elements.  
It is written as ∅ or {}

Important distinction:

- ∅ is an empty set
    
- {∅} is a set that contains the empty set
    

> [!note] ∅ ⊆ A for any set A. The empty set is always a subset of every set.

> [!quote] “An empty box is not the same as a box with an empty box inside it.” — _[[Richard Hammack]]_

> [!quote] “The empty set is the only set whose cardinality is zero.” — _[[Richard Hammack]]_

---

### [[Cardinality]] (in [[Book of Proof]] by [[Richard Hammack]])

**Cardinality** is the number of elements in a set, written |A|.

Examples:

- |{2, 4, 6}| = 3
    
- |∅| = 0
    

> [!note] For a finite set A, |A| equals the number of distinct elements in A.

---

### [[Special Sets]] (in [[Book of Proof]] by [[Richard Hammack]])

Commonly used sets in mathematics include:

- ℕ: Natural numbers = {1, 2, 3, ...}
    
- ℤ: Integers = {..., −3, −2, −1, 0, 1, 2, ...}
    
- ℚ: Rational numbers = {m/n : m, n ∈ ℤ, n ≠ 0}
    
- ℝ: Real numbers = all numbers on the number line
    
- ∅: The empty set
    

> [!note] Sets are not limited to numbers — they can contain symbols, ordered pairs, matrices, or even other sets.

---

### [[Set-Builder Notation]] (in [[Book of Proof]] by [[Richard Hammack]])

Set-builder notation allows us to define sets by a **property** rather than listing elements.

Format:  
**{expression : condition}**  
(read as “the set of all elements of the form _expression_ such that _condition_ holds”)

Examples:

- E = {2n : n ∈ ℤ} defines all even integers
    
- {x ∈ ℝ : x² = 4} = {−2, 2}
    

> [!note] The colon “:” in set-builder notation is often replaced with a vertical bar “|” by some authors.

---

### [[Absolute Value]] vs [[Cardinality]] (in [[Book of Proof]] by [[Richard Hammack]])

The symbol `| |` can mean different things:

- If applied to a number (like x), |x| means **absolute value**
    
- If applied to a set (like A), |A| means **cardinality**
    

Example:

- |−5| = 5
    
- |{a, b, c}| = 3
    

> [!note] Context determines whether vertical bars mean cardinality or absolute value.

---
## 1.2 The Cartesian Product

Tags: 

The **Cartesian product** of two sets A and B, written **A × B**, is the set of all **ordered pairs** (a, b) where **a ∈ A** and **b ∈ B**.

Example:  
If A = {1, 2} and B = {x, y}, then:  
A × B = {(1, x), (1, y), (2, x), (2, y)}

> [!note] Cartesian products allow us to pair elements from one set with elements of another, forming the foundation of coordinate systems.

---

### [[Ordered Pair]] (in [[Book of Proof]] by [[Richard Hammack]])

An **ordered pair** is a pair of elements (a, b), where:

- The first component comes from the first set (A)
    
- The second component comes from the second set (B)
    

Order matters:  
(2, 4) ≠ (4, 2) unless 2 = 4.

> [!note] Ordered pairs distinguish positions in space, sequences, and functions.

---

### [[Cartesian Product]] (in [[Book of Proof]] by [[Richard Hammack]])

Definition:  
**A × B = {(a, b) : a ∈ A and b ∈ B}**

It represents all possible pairings between elements of A and B.

> [!note] The number of elements in A × B equals |A| × |B| if A and B are finite.

---

### [[Cartesian Power]] (in [[Book of Proof]] by [[Richard Hammack]])

The **Cartesian power** of a set A, written Aⁿ, is the Cartesian product of A with itself n times.

Examples:

- A² = A × A = all ordered pairs (a₁, a₂)
    
- A³ = A × A × A = all triples (a₁, a₂, a₃)
    

Common spaces:

- ℝ² = all points in the 2D plane
    
- ℝ³ = all points in 3D space
    

> [!note] Cartesian powers are used in geometry, algebra, and analysis to describe higher-dimensional spaces.

> [!quote] “We use ℝ² and ℝ³ as the mathematical models for the two- and three-dimensional space in which we live.” — _[[Richard Hammack]]_

## 1.3 Subsets

Tags: #SetTheory

A set **A** is a **subset** of a set **B** (written **A ⊆ B**) if **every element** of A is also an element of B.

Examples:

- {1, 2} ⊆ {1, 2, 3} is **true**
    
- {1, 4} ⊆ {1, 2, 3} is **false**
    

Note:

- **Every set is a subset of itself**: A ⊆ A
    
- **The empty set** is a subset of every set: ∅ ⊆ A
    

> [!note] The empty set is a subset of all sets.

---

### [[Subset]] (in [[Book of Proof]] by [[Richard Hammack]])

Notation:  
A ⊆ B means: ∀x (if x ∈ A, then x ∈ B)

There are **two** subset symbols:

- A ⊆ B: A is a subset of B (possibly equal)
    
- A ⊂ B: A is a **proper subset** of B (A ⊆ B and A ≠ B
    

> [!note] A set with _n_ elements has exactly _2ⁿ_ subsets.

---

### [[Power Set]] (in [[Book of Proof]] by [[Richard Hammack]])

The **power set** of A, denoted **P(A)**, is the set of all subsets of A.

Example:  
If A = {1, 2}, then  
P(A) = {∅, {1}, {2}, {1, 2}}

Fact:  
If |A| = n, then |P(A)| = 2ⁿ

> [!note] The power set of A contains all combinations of its elements, including the empty set and A itself.

---
## 1.4 Power Sets

Tags: #SetTheory

The **power set** of a set A, written **P(A)**, is the set of **all subsets** of A.

Example:  
If A = {1, 2, 3}, then:

P(A) = {∅, {1}, {2}, {3}, {1, 2}, {1, 3}, {2, 3}, {1, 2, 3}}

This includes:

- The **empty set**
    
- Every **proper subset**
    
- The **set A itself**
    

> [!note] A power set always contains 2ⁿ elements if A has n elements.

---

### [[Power Set]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

Definition:  
**P(A) = {X : X ⊆ A}**

It contains every subset of A — regardless of size.

If |A| = n, then |P(A)| = 2ⁿ.

> [!note] The power set of even a small set can be surprisingly large. For example, a 10-element set has a power set with 1,024 subsets.

---

> [!quote] “Despite their similarity, we maintain that a matrix is not the same thing as a sequence of numbers.” — _[[Richard Hammack]]_

> [!quote] “P(ℝ²) contains every imaginable black-and-white image, function, or book ever written.” — _ [[Richard Hammack]] _
> 

---
## 1.5 Union, Intersection, Difference

Tags:

This section introduces three fundamental **set operations**: union, intersection, and set difference. These operations allow us to combine or compare sets logically and visually (via Venn diagrams in later sections).

---

### [[Union]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

The **union** of sets A and B, written **A ∪ B**, is the set of all elements that are in **A**, in **B**, or in **both**.

Example:  
If A = {1, 2} and B = {2, 3}, then  
A ∪ B = {1, 2, 3}

> [!note] Union is inclusive — elements appearing in either or both sets are included.

---

### [[Intersection]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

The **intersection** of sets A and B, written **A ∩ B**, is the set of all elements **common to both** A and B.

Example:  
If A = {1, 2} and B = {2, 3}, then  
A ∩ B = {2}

> [!note] Intersection focuses only on shared elements between sets.

---

### [[Set Difference]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

The **difference** of A and B, written **A − B**, is the set of all elements that are in A but **not** in B.

Example:  
If A = {1, 2, 3} and B = {2, 3}, then  
A − B = {1}

Note:

- A − B ≠ B − A in general
    
- A − B = A ∩ Bᶜ
    

> [!note] Set difference is not commutative — switching A and B can change the result.

---

> [!note] Union and intersection are both **Commutative** and **[[Associative]]** operations:
> 
> - A ∪ B = B ∪ A
>     
> - A ∩ B = B ∩ A
>     
> - (A ∪ B) ∪ C = A ∪ (B ∪ C)
>     
> - (A ∩ B) ∩ C = A ∩ (B ∩ C)


---


## 1.6 Complement

Tags: #SetTheory

The **complement** of a set A, written **Aᶜ**, is the set of all elements that are **not in A**, relative to some fixed **universal set** U.

Definition:  
**Aᶜ = U − A**

This means Aᶜ contains everything in U that is not in A.

> [!note] Set complements depend on the chosen universal set U, which must be specified or understood from context.

---

### [[Complement]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

If U is the universal set and A ⊆ U, then:  
**Aᶜ = {x ∈ U : x ∉ A}**

Example:  ![](data:image/webp;base64,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)

[[book_of_proof.pdf#page=32&rect=54,65,429,104&color=note|book_of_proof, p.20]]
Let U = {1, 2, 3, 4, 5} and A = {2, 4}, then  
Aᶜ = {1, 3, 5}

> [!note] A ∪ Aᶜ = U and A ∩ Aᶜ = ∅ — these are fundamental complement identities.

---

> [!note] The complement operation follows **[[De Morgan’s Laws]]** when combined with union and intersection:
> 
> - (A ∪ B)ᶜ = Aᶜ ∩ Bᶜ
>     
> - (A ∩ B)ᶜ = Aᶜ ∪ Bᶜ

## 1.7 Venn Diagrams

Tags: #venndiagrams

**Venn diagrams** are visual tools used to represent relationships between sets. Each set is shown as a circle within a rectangle that represents the **universal set**.

They are especially helpful for understanding operations like:

- [[Union]] (A ∪ B): shaded area includes everything in A or B or both
    
- [[Intersection]] (A ∩ B): shaded area includes only elements in both A and B
    
- [[Set Difference]] (A − B): shaded area includes elements in A but not in B
    
- [[Complement]] (Aᶜ): shaded area includes everything outside A
    

> [!note] Venn diagrams offer intuitive insight into abstract set relationships, especially when working with 2 or 3 sets.

---

> [!note] The full universal set is typically shown as a rectangle enclosing all the circles representing the individual sets.

> [!note] Venn diagrams become harder to read beyond three sets, but still convey valuable logic patterns in simpler cases.


## 1.8 Indexed Sets

Tags: #IndexedSets

An **indexed set** is a collection of sets, each labeled or associated with an **index** from another set.

This structure allows us to talk about entire families of sets at once — especially useful in unions, intersections, and sequences.

Example:  
Let A₁ = {1}, A₂ = {1, 2}, A₃ = {1, 2, 3}, etc.  
Then {A₁, A₂, A₃, ...} is an **indexed family of sets**, indexed by the natural numbers ℕ.

> [!note] Indexing provides structure when dealing with infinitely many sets or when naming each set individually would be impractical.

---

### [[Indexed Set]] (in [[Book of Proof]] by [[Richard Hammack]])

An indexed collection is written:  
**{Aᵢ : i ∈ I}**, where I is the **index set**, and each Aᵢ is a set.

- I could be finite (e.g. {1, 2, 3}) or infinite (e.g. ℕ)
    
- A₁, A₂, A₃, ... are referred to as an indexed family of sets
    

> [!note] The subscript "i" identifies each set Aᵢ according to its position or role in the collection.

---

### [[Indexed Union]] and [[Indexed Intersection]]

(in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

If {Aᵢ : i ∈ I} is an indexed family of sets:

- **⋃ Aᵢ** = the union over all Aᵢ (elements that appear in at least one Aᵢ)
    
- **⋂ Aᵢ** = the intersection over all Aᵢ (elements common to all Aᵢ)
    

Example:  
If Aₙ = {n, n+1} for n ∈ ℕ:

- ⋃ Aₙ = ℕ
    
- ⋂ Aₙ = ∅ (no element is in **every** Aₙ)
    

> [!note] Indexed operations generalize union and intersection beyond two or three sets — they’re especially useful in analysis and logic.


## 1.9 Sets That Are Number Systems

Tags: #NumberSystems

Certain sets of numbers are so foundational that they are treated as standard mathematical objects. These sets form the backbone of nearly all areas in mathematics, from arithmetic to analysis.

---

### [[Natural Numbers]] (in [[Book of Proof ]] by [[Richard Hammack]])

The **natural numbers**, denoted **ℕ**, are the positive whole numbers:  
**ℕ = {1, 2, 3, 4, ...}**

> [!note] Some authors include 0 in ℕ, but in this book ℕ begins with 1.

---

### [[Integers]] (in [[Book of Proof]] by [[Richard Hammack]])

The **integers**, denoted **ℤ**, include all whole numbers, positive and negative:  
**ℤ = {..., −3, −2, −1, 0, 1, 2, 3, ...}**

---

### [[Rational Numbers]] (in [[Book of Proof]] by [[Richard Hammack]])

The **rational numbers**, denoted **ℚ**, are all numbers that can be written as a **fraction** of integers:  
**ℚ = {m/n : m, n ∈ ℤ, n ≠ 0}**

These numbers **include**:

- Integers (e.g. 3 = 3/1)
    
- Finite decimals (e.g. 0.25 = 1/4)
    
- Repeating decimals (e.g. 0.333... = 1/3)
    

> [!note] Every integer is rational, but not every real number is rational.

---

### [[Real Numbers]] (in [[Book of Proof]] by [[Richard Hammack]])

The **real numbers**, denoted **ℝ**, include all possible points on the **number line**.  
They contain:

- All rational numbers
    
- All **irrational numbers** (e.g. √2, π, e)
    

> [!note] Irrational numbers are real but not rational — they cannot be written as exact fractions.

> [!quote] “We visualize the set ℝ of real numbers as an infinitely long number line.” — _[[Richard Hammack]]_

> [!quote] “ℚ ≠ ℝ, as √2 ∉ ℚ but √2 ∈ ℝ.” — _ [[Richard Hammack]] _


## 1.10 Russell’s Paradox

Tags: #SetTheory #RussellsParadox

**Russell’s Paradox** shows that not every rule defines a valid set. It arises when we consider sets that try to contain themselves.

Define the set:  
**R = {X : X ∉ X}**  
This is the set of all sets that **do not contain themselves**.

Now ask: **Does R contain itself?**

- If **R ∈ R**, then by definition **R ∉ R**
    
- If **R ∉ R**, then it **must be** in R  
    → This leads to a **logical contradiction**
    

> [!note] The paradox proves that naive set theory — where “any definable collection is a set” — leads to inconsistencies.

---

### [[Russell’s Paradox]] (in [[Book of Proof ]] by [[Richard Hammack]])

This paradox was discovered by **Bertrand Russell** in the early 20th century and was a major shock to foundational mathematics.

It prompted the development of **axiomatic set theories** like **Zermelo–Fraenkel set theory (ZF)**, where strict rules govern what counts as a valid set.

> [!note] Russell’s Paradox shows that unrestricted set definitions can produce contradictions if self-reference is allowed.

> [!quote] “Russell’s Paradox reveals that some collections, though logically definable, are too contradictory to be considered sets.” — _ [[Richard Hammack]] _
> 

# Chapter 2 — [[Logic]] | [[Book of Proof]] | [[Richard Hammack]]

> [!PDF|note] [[book_of_proof.pdf#page=46&selection=5,0,9,64&color=note|book_of_proof, p.34]]
> > Logic is a systematic way of thinking that allows us to parse the meanings of sentences and to deduce new information from old information.
## 2.1 Statements

Tags: #LogicalStatements

In mathematics, a **statement** is a sentence that is **unequivocally either true or false** — but not both.

Examples of valid statements:

- “2 + 2 = 4” → **true**
    
- “7 is an even number” → **false**
    

Not statements:

- “x + 2 = 5” (until x is specified)
    
- Questions, commands, or ambiguous phrases like “Close the door.”
    

> [!note] A sentence must have a clear truth value to qualify as a logical statement.

---

### [[Statement]] (in [[Book of Proof]] by [[Richard Hammack]])

A **statement** is a declarative sentence that has a **definite truth value** — it is either **true (T)** or **false (F)**.

This makes statements the foundation of all logical reasoning and proofs.

> [!quote] “In mathematics, every assertion must be unambiguously true or false.” — _[[Richard Hammack]]_


> [!PDF|yellow] [[book_of_proof.pdf#page=49&selection=192,0,243,1&color=yellow|book_of_proof, p.37]]
> > It is called Fermat’s last theorem after Pierre Fermat, a seventeenthcentury French mathematician who scribbled it in the margin of a book. R : For all numbers a, b, c, n ∈ N with n > 2, it is the case that an + bn 6 = cn.

> [!PDF|yellow] [[book_of_proof.pdf#page=49&selection=257,0,268,30&color=yellow|book_of_proof, p.37]]
> > Goldbach conjecture: S : Every even integer greater than 2 is a sum of two prime numbers.


## 2.2 And, Or, Not

Tags: #LogicalConnectives

Logical connectives allow us to **combine statements** and build more complex logical expressions. The three basic connectives are:

- **And** (conjunction)
    
- **Or** (disjunction)
    
- **Not** (negation)
    

Each connective has its own symbol and behavior defined through **truth values**.

---

### [[Conjunction]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

The **conjunction** of two statements P and Q is written **P ∧ Q**.  
It means **both P and Q are true**.

Truth table for P ∧ Q:

|P|Q|P ∧ Q|
|---|---|---|
|T|T|T|
|T|F|F|
|F|T|F|
|F|F|F|

> [!note] A conjunction is only true when **both** components are true.

---

### [[Disjunction]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

The **disjunction** of two statements P and Q is written **P ∨ Q**.  
It means **P or Q or both are true** (inclusive or).

Truth table for P ∨ Q:

|P|Q|P ∨ Q|
|---|---|---|
|T|T|T|
|T|F|T|
|F|T|T|
|F|F|F|

> [!note] Disjunction in formal logic is **inclusive** — it allows both P and Q to be true.

---

### [[Negation]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

The **negation** of a statement P is written **¬P** (or sometimes ~P).  
It means “**not P**”.

Truth table for ¬P:

|P|¬P|
|---|---|
|T|F|
|F|T|

> [!note] Negation reverses the truth value of a statement.

---

> [!quote] “The logical operations AND, OR, and NOT are fundamental to constructing compound statements.” — _ [[Richard Hammack]] _
> 

## 2.3 Conditional Statements

Tags: #ConditionalStatements

A **conditional statement** connects two statements in an **if–then** format. It asserts that if one statement (the hypothesis) is true, then another (the conclusion) must also be true.

---

### [[Conditional Statement]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

The conditional statement “**If P, then Q**” is written symbolically as **P → Q**.

- **P** is the **hypothesis** (also called the antecedent)
    
- **Q** is the **conclusion** (also called the consequent)
    

> [!note] A conditional is considered **true** in every case **except** when P is true and Q is false.

---

### Truth Table for P → Q

|P|Q|P → Q|
|---|---|---|
|T|T|T|
|T|F|F|
|F|T|T|
|F|F|T|

> [!note] A false hypothesis makes the conditional true, regardless of the conclusion — this can feel counterintuitive but is logically consistent.

---

### [[Implication]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

“P implies Q” and “If P, then Q” are logically equivalent.

These all express the same relationship:

- P → Q
    
- P implies Q
    
- If P, then Q
    
- Q is true whenever P is true
    

---

### Terminology Variants

These are common alternate forms of conditional statements:

- “P only if Q” means P → Q
    
- “Q whenever P” also means P → Q
    
- “Q is a necessary condition for P” means P → Q
    
- “P is a sufficient condition for Q” also means P → Q
    

> [!note] Interpreting conditional statements in English requires care — phrases like "only if" and "whenever" can reverse the apparent order.

---

> [!quote] “Mathematical logic insists on truth tables because our intuition about conditionals is often unreliable.” — _ [[Richard Hammack]]
> _




## 2.4 Converse, Contrapositive, and Biconditional

Tags: #LogicalEquivalence #Conditionals

This section explores how variations of conditional statements relate to one another in meaning and truth value.

---

### [[Converse]] (in [[Book of Proof ]] by [[Richard Hammack]])

The **converse** of a conditional **P → Q** is the statement **Q → P**.

Example:  
Original: If a number is even, then it is divisible by 2.  
Converse: If a number is divisible by 2, then it is even. (This happens to be true, but in general the converse may not be.)

> [!note] The truth of P → Q does not guarantee the truth of its converse Q → P.

---

### [[Contrapositive]] (in [[Book of Proof]] by [[Richard Hammack]])

The **contrapositive** of a conditional **P → Q** is **¬Q → ¬P**.

Example:  
Original: If n is even, then n² is even.  
Contrapositive: If n² is not even, then n is not even.

> [!note] A conditional and its contrapositive are **logically equivalent** — they always have the same truth value.

---

### [[Biconditional]] (in [[Book of Proof]] by [[Richard Hammack]])

A **biconditional** statement is written **P ↔ Q**, and means:  
**“P if and only if Q”** (abbreviated as “iff”)

This asserts that **P and Q are logically equivalent**:

- If P is true, then Q is true
    
- If Q is true, then P is true
    

Truth table for P ↔ Q:

|P|Q|P ↔ Q|
|---|---|---|
|T|T|T|
|T|F|F|
|F|T|F|
|F|F|T|

> [!note] A biconditional is true when **both statements have the same truth value**.

---

> [!quote] “The contrapositive is logically equivalent to the original statement, while the converse generally is not.” — _[[Richard Hammack]]_

## 2.5 Tautologies, Contradictions, Logical Equivalence

Tags: #LogicalEquivalence #Tautology #Contradiction

This section introduces three important classifications of compound logical statements based on their **truth tables**.

---

### [[Tautology]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

A **tautology** is a compound logical statement that is **always true**, no matter the truth values of its component statements.

Example:  
**P ∨ ¬P** is always true (this is the **Law of the Excluded Middle**)

> [!note] A tautology is like a universal truth in logic — it never fails regardless of inputs.

---

### [[Contradiction]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

A **contradiction** is a compound statement that is **always false**.

Example:  
**P ∧ ¬P** is always false — it asserts that P is both true and false simultaneously, which is impossible.

> [!note] A contradiction is false in every possible scenario — it is logically impossible.

---

### [[Logical Equivalence]] (in [[Book of Proof by Richard Hammack]] by [[Richard Hammack]])

Two statements **P** and **Q** are **logically equivalent** if **P ↔ Q is a tautology** — that is, P and Q always share the same truth value.

Notation:  
**P ≡ Q** means P and Q are logically equivalent.

Example:  
**¬(P ∨ Q) ≡ (¬P ∧ ¬Q)** (This is one of **De Morgan’s Laws**)

> [!note] Logical equivalence is the logical version of equality — it tells us that two statements behave identically in all cases.

---

> [!quote] “Tautologies and contradictions are extreme forms of compound statements — always true or always false.” — _[[Richard Hammack]]_
## 2.6 More Examples

Tags: #LogicalExamples #TruthTables

This section presents additional truth tables to deepen understanding of how compound statements behave under different combinations of truth values. It reinforces the ideas of **logical connectives** and **equivalence** introduced earlier.

---

### Example 1: ¬(P ∧ Q)

Truth table:

|P|Q|P ∧ Q|¬(P ∧ Q)|
|---|---|---|---|
|T|T|T|F|
|T|F|F|T|
|F|T|F|T|
|F|F|F|T|

This example shows that **¬(P ∧ Q)** is **not** logically equivalent to **¬P ∧ ¬Q**, but **is** equivalent to **¬P ∨ ¬Q** (by **De Morgan’s Law**).

---

### [[De Morgan's Laws]] (in [[Book of Proof]] by [[Richard Hammack]])

These two identities are fundamental for rewriting logical expressions:

- ¬(P ∧ Q) ≡ ¬P ∨ ¬Q
    
- ¬(P ∨ Q) ≡ ¬P ∧ ¬Q
    

> [!note] De Morgan’s Laws let us distribute negation across conjunctions and disjunctions in logical expressions.

---

### Example 2: (P → Q) ∧ (Q → P)

This compound statement represents **P ↔ Q**, the **biconditional**.

Truth table:

|P|Q|P → Q|Q → P|(P → Q) ∧ (Q → P)|
|---|---|---|---|---|
|T|T|T|T|T|
|T|F|F|T|F|
|F|T|T|F|F|
|F|F|T|T|T|

> [!note] This example proves that **P ↔ Q** is logically equivalent to **(P → Q) ∧ (Q → P)**.

---

### [[Truth Table]] (in [[Book of Proof]] by [[Richard Hammack]])

A **truth table** shows the truth value of a compound statement for all combinations of truth values of its components. It is the primary tool for testing **equivalence**, **validity**, and **logical behavior**.

> [!PDF|yellow] [[book_of_proof.pdf#page=63&selection=233,0,297,1&color=yellow|book_of_proof, p.51]]
> > Two pairs of logically equivalent statements in particular are significant enough to have a special name: DeMorgan’s laws. Fact 2.1 (DeMorgan’s Laws) 1. ∼ (P ∧ Q) = (∼ P) ∨ (∼ Q) 2. ∼ (P ∨ Q) = (∼ P) ∧ (∼ Q)

![[book_of_proof.pdf#page=64&rect=88,405,429,539&color=note|book_of_proof, p.52]]
![[book_of_proof.pdf#page=63&rect=168,274,361,331&color=note|book_of_proof, p.51]]

> [!quote] “By building a truth table, we can understand exactly how a statement behaves.” — _[[Richard Hammack]]_

## 2.7 Truth Tables for Compound Statements

Tags: #TruthTables #LogicalConnectives

**Truth tables** provide a systematic way to understand the behavior of compound logical statements by exhaustively listing all combinations of truth values.

---

![[book_of_proof.pdf#page=65&rect=80,166,452,229&color=note|book_of_proof, p.53]]


### [[Truth Table]] (in [[Book of Proof]] by [[Richard Hammack]])

A **truth table** evaluates a compound statement’s truth value under every possible combination of truth values for its components.

This is essential for:

- Testing **logical equivalence**
    
- Proving **tautologies** or **contradictions**
    
- Clarifying **compound conditionals**
    

> [!note] The number of rows in a truth table doubles with each additional variable:
> 
> - 2 statements → 4 rows
>     
> - 3 statements → 8 rows
>     
> - 4 statements → 16 rows
>     

---

### Example: Constructing a Truth Table for a Complex Expression

Given:  
**¬(P ∧ (Q ∨ ¬R))**

We evaluate this in a column-wise breakdown:

|P|Q|R|¬R|Q ∨ ¬R|P ∧ (Q ∨ ¬R)|¬(P ∧ (Q ∨ ¬R))|
|---|---|---|---|---|---|---|
|T|T|T|F|T|T|F|
|T|T|F|T|T|T|F|
|T|F|T|F|F|F|T|
|T|F|F|T|T|T|F|
|F|T|T|F|T|F|T|
|F|T|F|T|T|F|T|
|F|F|T|F|F|F|T|
|F|F|F|T|T|F|T|

> [!note] Break compound expressions down **column by column** using logical rules to construct the full truth table.

---

> [!quote] “Constructing truth tables is laborious but completely mechanical — just follow the rules.” — _[[Richard Hammack]]_
Here is the structured and annotated summary of **Section 2.8: More on Conditional Statements** from _[[Book of Proof]] by [[Richard Hammack]]_, formatted with topic links and quotes per your instructions.

## 📘 2.8 More on Conditional Statements

**Tags**: #ConditionalLogic #Implication #MathematicalLogic

This section elaborates on the nuances of conditional statements (those of the form **“If P, then Q”**) and addresses common logical confusions in interpreting them.

---

### 🔗 [[Conditional Statements]] (in [[Book of Proof]] by [[Richard Hammack]])

A **conditional statement** has the form:

> **P → Q**  
> “If P, then Q”

This section emphasizes **how to interpret** and **reason with** such statements beyond just their truth tables.

---

### 🔗 [[True Implications with False Premises]] (in [[Book of Proof]] by [[Richard Hammack]])

Students often struggle with statements where the hypothesis is false. A key logical principle is:

> A conditional statement is **true** when its hypothesis is **false**, regardless of the conclusion.

For example:

- “If 5 is even, then 2+2=5” is **true** because the hypothesis ("5 is even") is false.
    

> [!quote]  
> This may seem counterintuitive at first, but logic considers such a conditional statement to be true because it makes no false claim.  
> — [[Richard Hammack]]

---

### 🔗 [[Examples of Conditional Reasoning]] (in [[Book of Proof]] by [[Richard Hammack]])

**Examples from the text** help clarify:

|Statement|Reason It’s True|
|---|---|
|If 7 is even, then 3 > 5|The hypothesis is false, so the whole statement is **true**|
|If 2 = 2, then 3 = 4|The hypothesis is **true**, conclusion **false** → the statement is **false**|

This shows that **only one case** (true hypothesis, false conclusion) makes a conditional false.

---

### 🔗 [[Logical Equivalents and Contrapositives]] (in [[Book of Proof]] by [[Richard Hammack]])

The contrapositive of a statement is logically equivalent:

> Original:     P → Q  
> Contrapositive: ¬Q → ¬P

Understanding this is key to **proof writing**, especially in contrapositive proof techniques.

---

> [!quote]  
> It is good practice to try the contrapositive if the original implication seems hard to prove.  
> — [[Richard Hammack]]

---

## 📘 2.9 Translating English to Symbolic Logic

**Tags**: #SymbolicLogic #LogicTranslation #MathematicalLogic

Translating natural language into **symbolic logic** helps clarify meaning, eliminate ambiguity, and allow precise reasoning. This skill is crucial for formulating rigorous **proofs** and working with **logical statements** in mathematics.

---

### 🔗 [[Symbolic Logic]] (in [[Book of Proof]] by [[Richard Hammack]])

This section teaches how to systematically convert English statements into symbolic form using:

- **Logical connectives**: ∧, ∨, →, ↔, ¬
    
- **Quantifiers**: ∀ ("for all"), ∃ ("there exists")
    
- **Variables and predicates**: Represent nouns and properties/conditions.
    

Example:

> "If a number is even, then its square is even."  
> Let E(x)E(x) mean “x is even.”  
> Then:  
> **∀x ∈ ℤ**, E(x) → E(x²)

---

### 🔗 [[Logical Connectives]] (in [[Book of Proof]] by [[Richard Hammack]])

The process involves:

1. **Identifying** the statement's logical structure
    
2. **Assigning predicates** to properties and relations
    
3. **Choosing the domain**
    
4. **Using quantifiers** and logical symbols accordingly
    

Some common translation patterns:

- “All…” → ∀
    
- “Some…” or “There exists…” → ∃
    
- “If… then…” → →
    
- “Not…” → ¬
    
- “A number is odd and greater than 3”  
    → Odd(x)∧x>3\text{Odd}(x) \land x > 3
    

---

### 🔗 [[Examples of Translation]] (in [[Book of Proof]] by [[Richard Hammack]])

Here are a few sample translations from the section:

|English Sentence|Symbolic Translation|
|---|---|
|All cats are mammals.|∀x (Cat(x) → Mammal(x))|
|Some students are tired.|∃x (Student(x) ∧ Tired(x))|
|No dogs are reptiles.|∀x (Dog(x) → ¬Reptile(x))|
|If x is rational, then x is real.|Rational(x) → Real(x)|

---

### 🔗 [[Translation Tips]] (in [[Book of Proof]] by [[Richard Hammack]])

- Define your **predicates clearly**
    
- Use parentheses to avoid ambiguity
    
- Watch for **hidden conditionals** ("Only if", "Unless", etc.)
    
- Be cautious with **negations and quantifiers** – negating ∃ becomes ∀¬, and vice versa.
    

> [!quote]  
> The important thing in translating an English sentence into symbolic logic is to maintain the meaning, not just to mimic the words.  
> — [[Richard Hammack]]


---

## 📘 2.10 Negating Statements

**Tags**: #Negation #Logic #Quantifiers #SymbolicLogic

Negation is the process of stating that a statement is **not true**. In logic, **negating statements accurately** is essential when disproving claims, constructing contrapositives, or understanding logical structure.

---

### 🔗 [[Negation]] (in [[Book of Proof]] by [[Richard Hammack]])

To negate a statement, you don’t just add “not” — you must **reverse the entire logical structure**. This is especially important for **quantified statements**.

---

### 🔗 [[Negating Quantifiers]] (in [[Book of Proof]] by [[Richard Hammack]])

Negating **universal** and **existential** quantifiers:

|Original Statement|Negation|
|---|---|
|∀x, P(x)|∃x such that ¬P(x)|
|∃x, P(x)|∀x, ¬P(x)|

💡 To negate a “for all” claim, you only need **one counterexample**.  
To negate “there exists,” you must rule out **all** cases.

---

### 🔗 [[Negating Logical Connectives]] (in [[Book of Proof]] by [[Richard Hammack]])

Negating compound statements follows these equivalences (De Morgan's Laws and others):

|Statement|Negation|
|---|---|
|¬(P ∧ Q)|(¬P ∨ ¬Q)|
|¬(P ∨ Q)|(¬P ∧ ¬Q)|
|¬(P → Q)|(P ∧ ¬Q)|

These identities are crucial in rewriting the **negation of conditionals**.

---


> Original:"If all unicorns are green, then no dragons exist."  
> Let:

- U(x): x is a unicorn
    
- G(x): x is green
    
- D(x): x is a dragon
    
- E(x): x exists
    

Then the statement is:  
**(∀x)(U(x) → G(x)) → ¬∃x(D(x) ∧ E(x))**

Its negation becomes:  
**(∀x)(U(x) → G(x)) ∧ ∃x(D(x) ∧ E(x))**

So the negation says:

> “All unicorns are green **and** some dragon exists.”

---

> [!quote]  
> To negate a statement correctly, you must analyze its logical structure and apply the correct rules to reverse it.  
> — [[Richard Hammack]]

Here is the structured and annotated summary of **Section 2.11: Logical Inference** from _[[Book of Proof]] by [[Richard Hammack]]_, following your requested format with internal topic links and author quote formatting.

---

## 📘 2.11 Logical Inference

**Tags**: #Inference #Logic #RulesOfInference #Deduction

A **logical inference** is a reasoning step in which you deduce a new statement (the **conclusion**) from given statements (the **premises**) using **valid logical rules**.

This section focuses on the use of **rules of inference** in proving mathematical statements.

---

### 🔗 [[Logical Inference]] (in [[Book of Proof]] by [[Richard Hammack]])

Logical inference allows you to:

- Combine or manipulate known true statements
    
- Draw conclusions guaranteed to be true if the premises are true
    
- Form the **backbone of formal proofs**
    

---

### 🔗 [[Basic Rules of Inference]] (in [[Book of Proof]] by [[Richard Hammack]])

Key rules include:

|Name|Form|Meaning|
|---|---|---|
|**Modus Ponens**|P → Q, P ⇒ Q|If P implies Q and P is true, then Q is true|
|**Modus Tollens**|P → Q, ¬Q ⇒ ¬P|If P implies Q and Q is false, then P is false|
|**Hypothetical Syllogism**|P → Q, Q → R ⇒ P → R|Chain of implications|
|**Disjunctive Syllogism**|P ∨ Q, ¬P ⇒ Q|If one is false, the other must be true|
|**Simplification**|P ∧ Q ⇒ P|From both, infer one|
|**Conjunction**|P, Q ⇒ P ∧ Q|Combine two truths|
|**Addition**|P ⇒ P ∨ Q|Add disjunction|

Each rule **preserves truth**, so if you start from true premises, your conclusion will also be true.

---

### 🔗 [[Applying Inference in Proofs]] (in [[Book of Proof]] by [[Richard Hammack]])

These rules are used in:

- **Direct proofs**
    
- **Proofs by contradiction**
    
- **Proofs by contrapositive**
    

Understanding inference is essential for constructing sound, logical arguments.

> [!quote]  
> Every line of a formal proof must follow from previous lines using valid rules of inference.  
> — [[Richard Hammack]]

---
Here's the structured and annotated summary of **Section 2.12: An Important Note** from _[[Book of Proof]] by [[Richard Hammack]]_, with links and author quotes as per your format.

---

## 📘 2.12 An Important Note

**Tags**: #MathematicalWriting #Logic #ProofClarity

This brief but essential section offers practical advice on the **use of symbols vs. words** in mathematical writing. While symbolic logic is a **powerful tool for analysis**, it is not always the best format for formal proof writing.

---

### 🔗 [[Mathematical Writing]] (in [[Book of Proof]] by [[Richard Hammack]])

> Symbolic logic helps us understand the structure and validity of statements, but formal mathematical proofs should be written **in clear, grammatical English** — with symbols used sparingly and only when helpful.

Key points:

- **Use words to explain your reasoning**
    
- **Reserve symbols** (like ∀, ∃, ∧, →) for short expressions or clarity
    
- **Avoid long chains of symbols** in body text — this hinders readability
    
- Remember that **proofs are communication**, not just logic exercises
    

---

> [!quote]  
> Mathematical writing should read like English prose, not like strings of symbols.  
> — [[Richard Hammack]]

> [!quote]  
> You will find that writing mathematics in complete English sentences will help you understand your own reasoning more clearly.  
> — [[Richard Hammack]]



---
# Chapter 3  [[Counting]] | [[Book of Proof]] | [[Richard Hammack]]
## 📘 3.1 Lists

**Tags**: #Counting #Combinatorics #OrderedLists #Fundamentals

This section introduces the concept of **lists** as foundational to counting problems in combinatorics. A **list** is an ordered arrangement of items, where **order matters** and **repetition may or may not be allowed**.

---

### 🔗 [[List]] (in [[Book of Proof]] by [[Richard Hammack]])

A **list** is a sequence (ordered collection) of elements from a set.

- Unlike sets, **order is important**
    
- Repetition of elements **is allowed**, unless otherwise specified
    
- Lists are also referred to as **tuples** (e.g., 2-tuples, 3-tuples)
    

Example:

> The set {a, b} gives rise to these 2-lists (or ordered pairs):  
> (a, a), (a, b), (b, a), (b, b)

This is different from subsets or combinations, where order does **not** matter.

---

### 🔗 [[How Many Lists?]] (in [[Book of Proof]] by [[Richard Hammack]])

Given a set with nn elements, the number of **k-lists** (lists of length k) is:

> nkn^k (if repetition is allowed)

Because for each of the kk positions in the list, there are nn choices.

Example:

- From the set {1, 2, 3}, the number of 2-lists is 32=93^2 = 9
    
- Lists: (1,1), (1,2), (1,3), (2,1), (2,2), … up to (3,3)
    

---

> [!quote]  
> Lists are a natural way to think about ordered arrangements of elements, and they form the basis for most counting arguments.  
> — [[Richard Hammack]]

---

### 🧠 Summary Notes

- Use lists when **order matters**
    
- With repetition: use **nkn^k**
    
- Without repetition: see next section on **permutations** (3.4)
    

Here is the structured and annotated summary of **Section 3.2: The Multiplication Principle** from _[[Book of Proof]] by [[Richard Hammack]]_, using your formatting with links and a quote block.

---

## 📘 3.2 The Multiplication Principle

**Tags**: #Counting #MultiplicationPrinciple #Combinatorics #DecisionTree

The **Multiplication Principle** is one of the most fundamental ideas in counting. It tells us how to count the number of possible outcomes when making a sequence of choices.

---

### 🔗 [[Multiplication Principle]] (in [[Book of Proof]] by [[Richard Hammack]])

**The Principle**:

> If a task consists of **k steps**, and:
> 
> - the first step can be done in n1n_1 ways
>     
> - the second in n2n_2 ways
>     
> - ...
>     
> - the kthk^\text{th} step in nkn_k ways
>     
> 
> Then the total number of ways to complete the task is:
> 
> n1⋅n2⋅⋯⋅nkn_1 \cdot n_2 \cdot \dots \cdot n_k

---

### 🔗 [[Applications of the Multiplication Principle]] (in [[Book of Proof]] by [[Richard Hammack]])

**Examples**:

- Creating a 3-letter password using the letters A, B, C:
    
    - Each position has 3 options → total = 3⋅3⋅3=273 \cdot 3 \cdot 3 = 27
        
- Choosing an outfit:
    
    - 4 shirts × 3 pants × 2 shoes = 4⋅3⋅2=244 \cdot 3 \cdot 2 = 24 combinations
        

This principle is often visualized with a **decision tree** or **branching diagram**, where each choice branches into the next set of choices.

---

### 🔗 [[Important Notes]] (in [[Book of Proof]] by [[Richard Hammack]])

- Choices must be **independent**: the number of ways to perform a step should not depend on previous steps (unless you're accounting for that specifically).
    
- This rule generalizes to problems involving **lists, permutations, and counting cases**.
    

---

> [!quote]  
> The multiplication principle is the foundation of all counting. It underlies lists, permutations, combinations and just about every counting problem you will encounter.  
> — [[Richard Hammack]]

---

## 📘 3.3 The Addition and Subtraction Principles

**Tags**: #Counting #AdditionPrinciple #SubtractionPrinciple #Combinatorics

These two principles are used when counting outcomes from **distinct cases** or **overlapping categories**. They complement the multiplication principle when choices are made **either-or**, not in sequence.

---

### 🔗 [[Addition Principle]] (in [[Book of Proof]] by [[Richard Hammack]])

**The Addition Principle**:

> If a task can be done in **mm** ways or in **nn** ways (with no overlap),  
> Then the total number of ways to do it is:
> 
> M+nm + n

✅ Use when choices are **mutually exclusive** (disjoint sets).

**Example**:

- You can take 3 buses or 4 trains to school  
    → Total options = 3+4=73 + 4 = 7
    

---

### 🔗 [[Subtraction Principle]] (in [[Book of Proof]] by [[Richard Hammack]])

**The Subtraction Principle**:

> If there are NN total possibilities, and BB of them are **bad** (unwanted),  
> Then the number of **good** outcomes is:
> 
> N−BN - B

✅ Use when it’s easier to **count everything** and subtract what you don’t want.

**Example**:

- A 3-digit number using digits 1–9 (no zeros) = 9⋅9⋅9=7299 \cdot 9 \cdot 9 = 729
    
- How many do **not** include the digit 5?  
    → First compute total with no restriction, then subtract the ones with digit 5
    

---

### 🔗 [[Combining Principles]] (in [[Book of Proof]] by [[Richard Hammack]])

You can combine these methods in complex problems:

Example:

> Count the number of 3-digit numbers that are divisible by 5 or 7  
> Use:

- Count divisible by 5
    
- Count divisible by 7
    
- Subtract overlap (divisible by both 5 and 7 = divisible by 35)
    

So:

∣A∪B∣=∣A∣+∣B∣−∣A∩B∣|A ∪ B| = |A| + |B| - |A ∩ B|

This foreshadows the **Inclusion-Exclusion Principle** (covered in Section 3.7).

---

> [!quote]  
> Use the addition principle for “either-or” cases that don’t overlap. Use subtraction when it's easier to count everything and remove the unwanted parts.  
> — [[Richard Hammack]]

Here is the structured and annotated summary of **Section 3.4: Factorials and Permutations** from _ [[Book of Proof]] by [[Richard Hammack]] _, following your preferred format with internal topic links and author quote.

---

## 📘 3.4 Factorials and Permutations

**Tags**: #Factorial #Permutation #Counting #Combinatorics

This section introduces the **factorial function** and uses it to count the number of **permutations** — ordered arrangements — of elements without repetition.

---

### 🔗 [[Factorial]] (in [[Book of Proof]] by [[Richard Hammack]])

The **factorial** of a nonnegative integer nn is defined as:

N!=n⋅(n−1)⋅(n−2)⋯3⋅2⋅1 n! = n \cdot (n-1) \cdot (n-2) \cdots 3 \cdot 2 \cdot 1

By definition: **0!=10! = 1**

|n|n!|
|---|---|
|0|1|
|1|1|
|3|6|
|5|120|
|7|5040|

Factorials grow very rapidly and are fundamental in many counting problems.

---

### 🔗 [[Permutation]] (in [[Book of Proof]] by [[Richard Hammack]])

A **permutation** is an **ordered arrangement** of elements **without repetition**.

**Number of permutations of nn distinct items**:

N! N!

**Number of rr-permutations** from nn items (choosing and ordering r items from n):

P (n, r)=n! (n−r)! P (n, r) = \frac{n!}{(n - r)!}

This answers: “How many ways can I arrange r out of n things?”

---

### 🔗 [[Examples of Permutations]] (in [[Book of Proof]] by [[Richard Hammack]])

- All arrangements of ABC (3 letters): 3!=63! = 6  
    → ABC, ACB, BAC, BCA, CAB, CBA
    
- How many 3-digit numbers can be formed from digits 1–9 with no repeats?  
    → 9⋅8⋅7=P (9,3)=9! 6!=5049 \cdot 8 \cdot 7 = P (9, 3) = \frac{9!}{6!} = 504
    
- How many ways to seat 5 out of 10 students in a row?  
    → P (10,5)=10! 5!=30240 P (10, 5) = \frac{10!}{5!} = 30240
    

---

> [!quote]  
> Permutations count the number of ways to arrange things when order matters and repetition is not allowed.  
> — [[Richard Hammack]]

---
Here is the structured and annotated summary of **Section 3.5: Counting Subsets** from _ [[Book of Proof]] by [[Richard Hammack]] _, including topic links and a quote from the author.

---

## 📘 3.5 Counting Subsets

**Tags**: #Combinations #Subsets #BinomialCoefficient #Counting

This section explains how to count the number of **unordered selections** (subsets) of a given size from a larger set — in contrast to **permutations**, where order matters.

---

### 🔗 [[Combination]] (in [[Book of Proof]] by [[Richard Hammack]])

A **combination** is an **unordered selection** of items without repetition.

If you want to choose rr items from a set of nn distinct items, and order **does not matter**, the number of such subsets is:

(nr)=n!R! (n−r)!\binom{n}{r} = \frac{n!}{r! (n - r)!}

This value is called a **binomial coefficient** and is read as “n choose r”.

---

### 🔗 [[Examples of Counting Subsets]] (in [[Book of Proof]] by [[Richard Hammack]])

- How many 2-element subsets can you choose from {A, B, C, D}?  
    → (42)=4! 2! 2!=6\binom{4}{2} = \frac{4!}{2! 2!} = 6
    

Subsets: {A, B}, {A, C}, {A, D}, {B, C}, {B, D}, {C, D}

- Choosing 5 lottery numbers from 50 (order doesn’t matter):  
    → (505)=50! 5!⋅45!\binom{50}{5} = \frac{50!}{5! \cdot 45!}
    
- Number of subsets of size 0 to nn:
    
    ∑k=0 n (nk)=2 n\sum_{k=0}^{n} \binom{n}{k} = 2^n

This shows the **total number of subsets of a set with n elements** is 2 n 2^n, aligning with the definition of the **power set** (see [[Power Set]] in Section 1.4).

---

### 🔗 [[Key Difference: Permutations vs. Combinations]]

- Permutations: Order matters → P (n, r)=n! (n−r)! P (n, r) = \frac{n!}{(n - r)!}
    
- Combinations: Order does **not** matter → (nr)=n!R! (n−r)!\binom{n}{r} = \frac{n!}{r! (n - r)!}
    

---

> [!quote]  
> When order does not matter, you are counting combinations — subsets — not permutations.  
> — [[Richard Hammack]]
Here is the structured and annotated summary of **Section 3.6: Pascal’s Triangle and the Binomial Theorem** from _ [[Book of Proof]] by [[Richard Hammack]] _, including topic links and author quote formatting.

---

## 📘 3.6 Pascal’s Triangle and the Binomial Theorem

**Tags**: #BinomialTheorem #PascalTriangle #Combinatorics #Algebra

This section explores the beautiful connection between **binomial coefficients**, **algebra**, and **combinatorics** through **Pascal’s Triangle** and the **Binomial Theorem**.

---

### 🔗 [[Pascal's Triangle]] (in [[Book of Proof]] by [[Richard Hammack]])

Pascal’s Triangle is a triangular array of numbers where:

- Each row corresponds to the coefficients of (a+b) n (a + b)^n
    
- Each number is the **sum of the two directly above it**
    
- The rthr^\text{th} entry in row nn is (nr)\binom{n}{r}
    

**Structure**:

```
         1
       1   1
     1   2   1
   1  3   3   1
 1  4   6   4   1
```

🔸 Each row gives the **coefficients** of (a+b) n (a + b)^n for increasing nn.

---

### 🔗 [[Binomial Theorem]] (in [[Book of Proof]] by [[Richard Hammack]])

The **Binomial Theorem** tells you how to expand (a+b) n (a + b)^n for any nonnegative integer nn:

(a+b) n=∑r=0 n (nr) an−rbr (a + b)^n = \sum_{r=0}^{n} \binom{n}{r} a^{n-r} b^r

**Example**:

(a+b) 3=(30) a 3 b 0+(31) a 2 b 1+(32) a 1 b 2+(33) a 0 b 3 (a + b)^3 = \binom{3}{0}a^3 b^0 + \binom{3}{1}a^2 b^1 + \binom{3}{2}a^1 b^2 + \binom{3}{3}a^0 b^3 =a 3+3 a 2 b+3 ab 2+b 3= a^3 + 3 a^2 b + 3 ab^2 + b^3

This gives a direct algebraic use of **combinatorial counting** via **(nr)\binom{n}{r}**.

---

### 🔗 [[Combinatorial Interpretation]] (in [[Book of Proof]] by [[Richard Hammack]])

- The coefficient (nr)\binom{n}{r} counts how many ways to choose rr b’s (and thus n−rn-r a’s) when expanding (a+b) n (a + b)^n
    
- Every term in the expansion corresponds to a **subset selection** (combination)
    

> [!quote]  
> The Binomial Theorem connects algebra with combinatorics by interpreting the expansion of (a+b) n (a + b)^n as a sum over combinations.  
> — [[Richard Hammack]]

---
Here is the structured and annotated summary of **Section 3.7: The Inclusion-Exclusion Principle** from _ [[Book of Proof]] by [[Richard Hammack]] _, with topic links and quote formatting as requested.

---

## 📘 3.7 The Inclusion-Exclusion Principle

**Tags**: #Counting #InclusionExclusion #OverlappingSets #SetTheory

This section introduces the **Inclusion-Exclusion Principle**, a method used to accurately count the number of elements in **unions of overlapping sets** — by adjusting for **double counting**.

---

### 🔗 [[Inclusion-Exclusion Principle]] (in [[Book of Proof]] by [[Richard Hammack]])

### 🔹 For Two Sets:

If AA and BB are finite sets, then:

∣A∪B∣=∣A∣+∣B∣−∣A∩B∣|A \cup B| = |A| + |B| - |A \cap B|

You subtract the overlap to avoid **double counting** the elements in both sets.

**Example**:

- Let AA be students taking math (30 students)
    
- Let BB be students taking science (25 students)
    
- Let ∣A∩B∣=10|A \cap B| = 10
    

Then:

∣A∪B∣=30+25−10=45|A \cup B| = 30 + 25 - 10 = 45

---

### 🔹 For Three Sets:

If AA, BB, and CC are finite sets:

∣A∪B∪C∣=∣A∣+∣B∣+∣C∣−∣A∩B∣−∣A∩C∣−∣B∩C∣+∣A∩B∩C∣|A \cup B \cup C| = |A| + |B| + |C| - |A \cap B| - |A \cap C| - |B \cap C| + |A \cap B \cap C|

This adds up all the sizes, subtracts the pairwise overlaps, and then **re-adds** the triple overlap (which was subtracted too many times).

---

### 🔗 [[Applications of Inclusion-Exclusion]] (in [[Book of Proof]] by [[Richard Hammack]])

Typical problems:

- Counting how many people like **at least one** of multiple options
    
- Finding how many numbers in a range are divisible by 3 or 5 (or both)
    
- Problems involving **"either/or/both"** logic
    

---

> [!quote]  
> The inclusion-exclusion principle corrects for overcounting by carefully subtracting and adding overlaps among sets.  
> — [[Richard Hammack]]

---

Here is the structured and annotated summary of **Section 3.8: Counting Multisets** from _ [[Book of Proof]] by [[Richard Hammack]] _, formatted with internal links and a quote block.

---

## 📘 3.8 Counting Multisets

**Tags**: #Multisets #Counting #Combinatorics #RepetitionAllowed

This section introduces **multisets**, which are collections where **repetition is allowed** and **order does not matter**. It explains how to count the number of such combinations using a classic **stars-and-bars** method.

---

### 🔗 [[Multisets]] (in [[Book of Proof]] by [[Richard Hammack]])

A **multiset** is like a set, except:

- Elements **can repeat**
    
- **Order still doesn’t matter**
    

**Example**:  
From set {A, B, C}, the multiset {A, A, C} is valid.  
This differs from permutations or regular subsets.

---

### 🔗 [[Counting r-Combinations with Repetition]] (in [[Book of Proof]] by [[Richard Hammack]])

The number of **multisets** of size rr that can be formed from a set of nn distinct elements is:

(n+r−1 r)\binom{n + r - 1}{r}

This is known as the **stars-and-bars formula**, derived from imagining:

- Rr stars (representing selections)
    
- N−1 n - 1 dividers (bars) separating item types
    

---

### 🔗 [[Example of Multiset Counting]] (in [[Book of Proof]] by [[Richard Hammack]])

**Example**:  
How many ways can you choose 5 fruits from 3 types (apple, banana, cherry), allowing repeats?

Answer: (3+5−15)=(75)=21\text{Answer: } \binom{3 + 5 - 1}{5} = \binom{7}{5} = 21

This counts all combinations like:  
{apple, apple, banana, banana, cherry}, etc.

---

### 🔗 [[Contrast with Regular Combinations]] (see [[Section 3.5]])

|Type|Order Matters?|Repeats Allowed?|Formula|
|---|---|---|---|
|Permutations|✅|❌|P (n, r) P (n, r)|
|Combinations|❌|❌|(nr)\binom{n}{r}|
|Multisets|❌|✅|(n+r−1 r)\binom{n + r - 1}{r}|

---

> [!quote]  
> A multiset allows repetition, and counting them requires different reasoning than sets or permutations.  
> — [[Richard Hammack]]

---
Here is the structured and annotated summary of **Section 3.9: The Division and Pigeonhole Principles** from _[[Book of Proof]] by [[Richard Hammack]]_, formatted with internal topic links and quote blocks as requested.

---

## 📘 3.9 The Division and Pigeonhole Principles

**Tags**: #Counting #DivisionPrinciple #PigeonholePrinciple #Combinatorics

This section presents two classic tools in combinatorics:

- The **Division Principle**: for counting grouped outcomes
    
- The **Pigeonhole Principle**: for proving existence of repetitions
    

---

### 🔗 [[Division Principle]] (in [[Book of Proof]] by [[Richard Hammack]])

**The Division Principle** is used when outcomes are grouped into **equivalent classes** or **repeated patterns**.

> If a procedure counts each outcome **k times**, then:
> 
> Number of distinct outcomes=Nk\text{Number of distinct outcomes} = \frac{N}{k}

Where:

- NN = total number of **labeled or repeated** arrangements
    
- kk = number of times each distinct object is counted
    

---

**Examples**:

- Counting unordered pairs (a, b) where order doesn't matter:
    
    - Total ordered pairs: (n2)⋅2=N\binom{n}{2} \cdot 2 = N
        
    - Divide by 2 to correct for symmetry
        
- Counting arrangements of the letters in "LEVEL":
    
    - Total = 5!2!⋅2!\frac{5!}{2! \cdot 2!} (because of repeated Ls and Es)
        

---

### 🔗 [[Pigeonhole Principle]] (in [[Book of Proof]] by [[Richard Hammack]])

**Basic Form**:

> If you place more than nn objects into nn containers, then **at least one container holds more than one object**.

**Formal statement**:  
If n+1n + 1 or more objects are placed in nn boxes,  
→ At least one box contains **2 or more** objects.

---

**Generalized Form**:

> If NN objects are placed into kk boxes,  
> then some box contains at least:
> 
> ⌈Nk⌉\left\lceil \frac{N}{k} \right\rceil

objects.

---

### 🔗 [[Examples of Pigeonhole Principle]] (in [[Book of Proof]] by [[Richard Hammack]])

- Among **13 people**, at least **2 share a birth month** (12 months → 13 people)
    
- Among **27 socks** in 4 colors, at least one color has **7 socks**  
    → ⌈274⌉=7\left\lceil \frac{27}{4} \right\rceil = 7
    

Used frequently in:

- Existence proofs
    
- Problems showing **repetition is unavoidable**
    
- Bounds on overlaps or collisions
    

---

> [!quote]  
> The pigeonhole principle is often used to prove that something must happen, even if you don’t know exactly when or where.  
> — [[Richard Hammack]]

---

## 📘 3.10 Combinatorial Proof

**Tags**: #Combinatorics #ProofByCounting #DoubleCounting #IdentityProof

This section introduces the technique of **combinatorial proof**, where a mathematical identity is proven by **counting the same thing in two different ways** — a powerful and elegant reasoning tool in discrete mathematics.

---

### 🔗 [[Combinatorial Proof]] (in [[Book of Proof]] by [[Richard Hammack]])

A **combinatorial proof** does not use algebra or calculus.  
Instead, it shows that **two expressions count the same set of outcomes**, just from different perspectives.

**Key idea**:

> Prove A=BA = B by interpreting both AA and BB as the count of the same collection.

---

### 🔗 [[Examples of Combinatorial Identities]] (in [[Book of Proof]] by [[Richard Hammack]])

#### Example 1:

(nr)=(nn−r)\binom{n}{r} = \binom{n}{n - r}

✔ Left side: choose **r** people from **n**  
✔ Right side: choose the **(n−r)** who are **not** selected

> Both expressions count the same subsets → proven combinatorially.

---

#### Example 2:

∑k=0n(nk)=2n\sum_{k = 0}^{n} \binom{n}{k} = 2^n

✔ Left side: sum of all subsets of size 0 to n  
✔ Right side: total number of all subsets of an nn-element set

This ties back to the **power set** in Section 1.4.

---

#### Example 3:

r⋅(nr)=n⋅(n−1r−1)r \cdot \binom{n}{r} = n \cdot \binom{n - 1}{r - 1}

✔ LHS: Choose a team of size rr, then choose a **captain**  
✔ RHS: First pick the **captain** (n options), then choose the other r−1r-1 teammates

---

> [!quote]  
> A combinatorial proof reveals that two seemingly different formulas are just two ways of counting the same set of outcomes.  
> — [[Richard Hammack]]

---

### 🧠 Why Combinatorial Proofs Matter

- Deepen understanding of **why** identities hold
    
- No algebraic manipulation needed
    
- Builds logical reasoning through interpretation
    

---
# Chapter 4 | [[Direct Proof]] | [[Book of Proof]] | [[Richard Hammack]] 

> [!PDF|note]  
> This section introduces the concept of a **theorem** — a central object in mathematics — and explains how mathematicians structure and interpret such statements before attempting to prove them.

---

## 📘 4.1 Theorems

**Tags**: #Theorem #ProofStructure #ConditionalStatements #MathematicalReasoning

A **theorem** is a **mathematical statement that has been proven to be true** using logic and previously established results (like definitions, axioms, or earlier theorems).

---

### 🔗 [[Theorem]] (in [[Book of Proof]] by [[Richard Hammack]])

A theorem often takes the **conditional form**:

> If PP, then QQ  
> Here, PP is the **hypothesis**, and QQ is the **conclusion**.

To prove a theorem, we must **assume the hypothesis is true** and then use logical reasoning to show the conclusion must also be true.

---

### 🔗 [[Parts of a Theorem]] (in [[Book of Proof]] by [[Richard Hammack]])

- **Hypothesis (or assumptions):** What you are given or allowed to assume
    
- **Conclusion (or claim):** What you must demonstrate follows from the hypothesis
    

Sometimes the hypothesis is implied or embedded in the phrasing.  
For example:

> “All even numbers are divisible by 2”  
> Can be rewritten logically as:  
> “If a number is even, then it is divisible by 2”

---

### 🔗 [[Terminology Around Theorems]] (in [[Book of Proof]] by [[Richard Hammack]])

Other named results include:

- **Lemma**: A “helper” theorem used in proving another theorem
    
- **Corollary**: A result that follows easily from a previously proven theorem
    
- **Proposition**: A result of lesser importance than a full theorem
    

While these labels differ in emphasis or importance, **all are proven results**.

---

> [!quote]  
> Theorems are the lifeblood of mathematics, and the process of proving them is what gives mathematics its logical foundation.  
> — [[Richard Hammack]]

---

> [!PDF|note]  
> This section emphasizes the critical role of **precise definitions** in mathematics and explains how to use them effectively in proofs and reasoning. Definitions are not suggestions — they are the foundation of logical clarity.

---

## 📘 4.2 Definitions

**Tags**: #Definitions #MathematicalPrecision #ProofWriting #LanguageOfMath

In mathematics, a **definition** precisely specifies the meaning of a term or concept. Definitions are **not negotiable**, and their role is central to both **understanding** and **constructing proofs**.

---

### 🔗 [[Definition]] (in [[Book of Proof]] by [[Richard Hammack]])

A **definition** tells you **exactly what it means** for something to satisfy a certain property.

- Definitions are **agreed-upon conventions**, not theorems.
    
- They are **not proved** — they are accepted and then **used to build** mathematical arguments.
    

**Example**:

> An integer nn is even if there exists an integer kk such that n=2kn = 2k.

This becomes your **tool** in proofs involving even numbers — not something to question or alter.

---

### 🔗 [[Using Definitions in Proofs]] (in [[Book of Proof]] by [[Richard Hammack]])

You must use definitions:

- **Exactly as written**
    
- **Explicitly** in your reasoning
    
- **Early** in the proof, especially when unpacking hypotheses
    

**Incorrect**:

> “Even numbers are numbers that can be divided by 2”  
> ✅ Instead, use:  
> “nn is even ⇔ n=2kn = 2k for some integer kk”

Precision avoids ambiguity — mathematical logic **does not tolerate vagueness**.

---

> [!quote]  
> The key to writing good proofs is to know your definitions and use them. In fact, this is often all you need to get started.  
> — [[Richard Hammack]]

---
Here is the structured and annotated summary of **Section 4.3: Direct Proof** from _[[Book of Proof]] by [[Richard Hammack]]_, with the **> [!PDF|note]** block as requested.

---

> [!PDF|note]  
> This section introduces the **direct proof method**, one of the most fundamental and widely used techniques in mathematical reasoning. It shows how to prove statements of the form “If PP, then QQ” by logically deriving the conclusion from the hypothesis.

---

## 📘 4.3 Direct Proof

**Tags**: #DirectProof #ProofTechnique #ConditionalStatement #LogicInPractice

A **direct proof** is a logical method that begins with an assumption that the hypothesis PP is true, and through clear, logical steps, establishes the truth of the conclusion QQ.

---

### 🔗 [[Direct Proof]] (in [[Book of Proof]] by [[Richard Hammack]])

The typical target for a direct proof is a conditional statement:

> If PP, then QQ

To construct a direct proof:

1. **Assume** the hypothesis PP is true.
    
2. **Use definitions, algebra, known facts**, and logical reasoning.
    
3. **Arrive at** the conclusion QQ.
    

---

 🔗Example of a Direct Proof

**Theorem**: If nn is an even integer, then n2n^2 is even.

**Proof**:

- Assume nn is even → n=2kn = 2k for some k∈Zk \in \mathbb{Z}
    
- Then n2=(2k)2=4k2=2(2k2)n^2 = (2k)^2 = 4k^2 = 2(2k^2), which is even
    
- ✅ Conclusion follows from definition of evenness
    

This illustrates the general format:

- Start with the hypothesis
    
- Plug in known definitions
    
- Do algebra or logic
    
- End with the conclusion
    

---

 🔗Tips for Writing Direct Proofs

- **Know your definitions**: These are often the only tools you need
    
- **Write in full sentences**: Proofs are arguments, not equations
    
- Don’t just state facts — **connect the dots** clearly
    
- Aim for **clarity and logic**, not cleverness
    

---

> [!quote]  
> Direct proof is often the simplest and clearest way to establish a result. It follows the logic of the statement: assume the hypothesis and show the conclusion.  
> — [[Richard Hammack]]
Here is the structured and annotated summary of **Section 4.4: Proof by Cases** from _[[Book of Proof]] by [[Richard Hammack]]_, formatted with your requested **> [!PDF|note]** block and study note structure.

---

> [!PDF|note]  
> This section introduces the **proof by cases** technique, which is useful when the hypothesis or domain naturally splits into **distinct, exhaustive scenarios**. You prove the conclusion separately in each case to show that it holds in all possible situations.

---

## 📘 4.4 Proof by Cases

**Tags**: #ProofByCases #CaseAnalysis #Logic #ExhaustiveReasoning

A **proof by cases** is a method in which you break the argument into multiple parts, each corresponding to a different scenario. You then prove the conclusion in **each case individually**.

---

### 🔗 [[Proof by Cases]] (in [[Book of Proof]] by [[Richard Hammack]])

Use proof by cases when:

- The hypothesis can lead to **multiple logical paths**
    
- The domain is **naturally divided** (e.g., even vs. odd, positive vs. negative)
    
- The statement must be proven true in **all possible cases**
    

**Structure**:

1. Identify **distinct, exhaustive cases**
    
2. Prove the conclusion holds **in each case**
    
3. Conclude that the result is universally valid
    

---

### 🔗 [[Example of Proof by Cases]] (in [[Book of Proof]] by [[Richard Hammack]])

**Theorem**:  
For any integer nn, n2+nn^2 + n is even.

**Proof**:  
We consider two cases:

**Case 1**: nn is even → n=2kn = 2k  
Then n2+n=(2k)2+2k=4k2+2k=2(2k2+k)n^2 + n = (2k)^2 + 2k = 4k^2 + 2k = 2(2k^2 + k) → even

**Case 2**: nn is odd → n=2k+1n = 2k + 1  
Then n2+n=(2k+1)2+(2k+1)=4k2+6k+2=2(2k2+3k+1)n^2 + n = (2k + 1)^2 + (2k + 1) = 4k^2 + 6k + 2 = 2(2k^2 + 3k + 1) → even

✅ In both cases, the result is even → Therefore, the theorem is true for all n∈Zn \in \mathbb{Z}

---
When to Use This Method

Choose proof by cases when:

- The structure of the problem splits into **clear alternatives**
    
- A **unified argument is difficult**, but case-by-case logic is manageable
    
- You can show all cases cover **every possibility**
    

> Be sure your cases are **mutually exclusive and collectively exhaustive**.

---

> [!quote]  
> Proof by cases is like covering all branches of a decision tree — if the conclusion holds in every branch, it holds overall.  
> — [[Richard Hammack]]

---
> [!PDF|note]  
> This section refines the technique of proof by cases, showing how to handle **multiple similar cases** efficiently. Instead of repeating the same argument over and over, you can prove one case in full and summarize the others — as long as they follow the same logic.

---

## 📘 4.5 Similar Cases

**Tags**: #ProofByCases #Efficiency #MathematicalWriting #Clarity

When using **proof by cases**, if multiple cases are **structurally identical**, you don’t need to fully write out each one. You can prove one in detail and **state that the others follow similarly** — provided they truly are similar.

---

### 🔗 [[Handling Similar Cases]] (in [[Book of Proof]] by [[Richard Hammack]])

**Example Situation**:  
You’re proving a statement for all integers n∈{−3,−2,−1,0,1,2,3}n \in \{-3, -2, -1, 0, 1, 2, 3\}n∈{−3,−2,−1,0,1,2,3}

Rather than proving all 7 cases individually:

- You might notice the proof works the same way for all **non-negative integers**
    
- And similarly for all **negative integers**
    

So, you break it into **two logical cases** instead of seven:

1. Case 1: n≥0n \geq 0n≥0
    
2. Case 2: n<0n < 0n<0
    

Then within each case, you only prove the representative logic **once**.

---

### 🔗 [[Guidelines for Using Similar Cases]] (in [[Book of Proof]] by [[Richard Hammack]])

✔ You **must** prove at least **one full case**  
✔ Make sure other cases genuinely follow the **same structure**  
✔ Do **not** skip a case just because it seems “obvious”  
✔ Always specify that the other cases are **handled the same way**

This keeps your proof:

- Concise
    
- Focused
    
- Readable
    
- Still rigorous
    

---

> [!quote]  
> Mathematicians value elegance and brevity, but not at the expense of clarity or logical completeness.  
> — [[Richard Hammack]]
Would you like to continue with **Section 4.5: Similar Cases**, or would a summary sheet comparing **direct proof** and **proof by cases** be helpful first?


> [!PDF|note]  
> This chapter introduces the method of **proof by contrapositive**, a powerful alternative to direct proof. It’s particularly useful when the conclusion of a statement is hard to prove directly but its **negation is easier to work with**.

---

## 📘 Chapter 5: Proof by Contrapositive

**Tags**: #ContrapositiveProof #LogicalEquivalence #ProofTechnique #Negation

Here is the structured and annotated summary of **Section 5.1: Proof by Contrapositive** from _[[Book of Proof]] by [[Richard Hammack]]_, formatted with your requested **> [!PDF|note]** block and internal topic links.

---

> [!PDF|note]  
> This section introduces the **contrapositive proof technique**, a powerful alternative to direct proof. Instead of proving “If PP, then QQ” directly, you prove the logically equivalent statement: “If not QQ, then not PP”.

---

## 📘 5.1 Proof by Contrapositive

**Tags**: #Contrapositive #ProofTechnique #LogicEquivalence #IndirectProof

The **contrapositive** of a conditional statement is **logically equivalent** to the original.  
This method is especially helpful when the **direct path from PP to QQ** is unclear, but it’s easier to show that **¬Q\neg Q implies ¬P\neg P**.

---

### 🔗 [[Contrapositive]] (in [[Book of Proof]] by [[Richard Hammack]])

The contrapositive of:

> If PP, then QQ  
> is:  
> If ¬Q\neg Q, then ¬P\neg P

These two are logically equivalent:

P→Q≡¬Q→¬PP \rightarrow Q \equiv \neg Q \rightarrow \neg P

✔ If one is true, so is the other  
✔ So, proving the contrapositive **proves the original statement**

---

### 🔗 [[Example of Contrapositive Proof]] (in [[Book of Proof]] by [[Richard Hammack]])

**Theorem**:  
If n2n^2 is even, then nn is even.

**Contrapositive**:  
If nn is odd, then n2n^2 is odd.

**Proof**:

- Let n=2k+1n = 2k + 1 (odd)
    
- Then n2=(2k+1)2=4k2+4k+1=2(2k2+2k)+1n^2 = (2k + 1)^2 = 4k^2 + 4k + 1 = 2(2k^2 + 2k) + 1
    
- So n2n^2 is odd
    
- ✅ Contrapositive is proven → original statement is true
    

---

### 🔗 [[When to Use Contrapositive Proofs]] (in [[Book of Proof]] by [[Richard Hammack]])

Use this method when:

- The **hypothesis is difficult to start from**, but
    
- The **negation of the conclusion** leads more easily to the **negation of the hypothesis**
    

This is often the case with statements about **divisibility**, **parity**, or **logical conditions**.

---

> [!quote]  
> A contrapositive proof lets you prove “If P, then Q” by showing that “If not Q, then not P.” This often makes the reasoning simpler and clearer.  
> — [[Richard Hammack]]

---

Here is the structured and annotated summary of **Section 5.2: Examples Using Contrapositive Proof** from _[[Book of Proof]] by [[Richard Hammack]]_, with your requested **> [!PDF|note]** block and internal links.

---

> [!PDF|note]  
> This section applies the contrapositive proof technique to real theorems, showing how and why it can be more effective than direct proof — especially in cases involving properties like parity or divisibility.

---

## 📘 5.2 Examples Using Contrapositive

**Tags**: #Contrapositive #ProofExamples #Parity #Divisibility #IndirectProof

This section demonstrates **how to prove theorems** using the **contrapositive method**. Each example shows why the contrapositive approach is simpler or more natural than a direct one.

---

### 🔗 [[Example 1]] (in [[Book of Proof]] by [[Richard Hammack]])

**Theorem**:  
If n2n^2 is even, then nn is even.

✅ Direct proof is tricky because starting with n2n^2 doesn’t give an easy path to nn.  
🔁 Contrapositive:

> If nn is odd, then n2n^2 is odd.

**Proof**:

- Let n=2k+1n = 2k + 1
    
- Then n2=4k2+4k+1=2(2k2+2k)+1n^2 = 4k^2 + 4k + 1 = 2(2k^2 + 2k) + 1
    
- So n2n^2 is odd
    
- ✅ Contrapositive proven → Theorem holds
    

---

### 🔗 [[Example 2]] (in [[Book of Proof]] by [[Richard Hammack]])

**Theorem**:  
If a2a^2 is divisible by 3, then aa is divisible by 3.

Again, proving directly is non-obvious.  
🔁 Contrapositive:

> If aa is **not** divisible by 3, then a2a^2 is **not** divisible by 3.

**Proof**:

- If aa is not divisible by 3, then a≡1a \equiv 1 or 2mod  32 \mod 3
    
- Then a2≡1mod  3a^2 \equiv 1 \mod 3 or 4≡1mod  34 \equiv 1 \mod 3
    
- In both cases, a2≢0mod  3a^2 \not\equiv 0 \mod 3
    
- So a2a^2 is not divisible by 3
    
- ✅ Contrapositive holds → Original statement is true
    

---

### 🔗 [[Strategy Insight]] (in [[Book of Proof]] by [[Richard Hammack]])

Why use contrapositive here?

- You can **plug in the assumption more naturally**
    
- You can use **modular arithmetic** or **definitions directly**
    
- The logical flow becomes **clearer and more elegant**
    

---

> [!quote]  
> Some theorems are not easily attacked head-on. Turning the statement around — by proving the contrapositive — often simplifies the process.  
> — [[Richard Hammack]]

---

Would you like to continue with **Chapter 6: Proof by Contradiction**, or receive a quick visual summary of all three indirect proof techniques (contrapositive, contradiction, cases)?

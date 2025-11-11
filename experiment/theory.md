# Theory: Syntax and Inference in Propositional Logic

## Introduction: The Language of Logic

Welcome to the fascinating world of propositional logic, where we transform everyday reasoning into precise mathematical statements! Just as we use grammar rules to construct meaningful sentences in English, propositional logic provides us with formal rules to construct and analyze logical arguments.

Think of propositional logic as the DNA of reasoning. Every complex argument, from philosophical debates to computer algorithms, can be broken down into these fundamental logical building blocks. This system was first developed by ancient Greek philosophers and has remained virtually unchanged for over 2000 years—a testament to its power and elegance.

### What Are Propositions?

A **proposition** is simply a statement that is either true or false—no middle ground allowed! Consider these examples:

**Valid Propositions:**
- "The sky is blue" (True)
- "2 + 2 = 5" (False)
- "It will rain tomorrow" (Either true or false, but not both)
- "All cats are mammals" (True)

**NOT Propositions:**
- "Hello there!" (A greeting, not true or false)
- "What time is it?" (A question)
- "Please close the door" (A command)
- "x + 5 = 10" (Contains a variable; truth depends on the value of x)

The beauty of propositional logic lies in its ability to combine simple propositions into complex ones, just like combining LEGO blocks to build elaborate structures.

## The Building Blocks: Atomic and Compound Propositions

### Atomic Propositions: The Simplest Form

An **atomic proposition** is like a fundamental particle in physics—it cannot be broken down into simpler logical components. We represent these using capital letters:

- **A**: "Alice is a student"
- **B**: "Bob likes pizza"
- **C**: "The library is open"
- **D**: "It is raining"

We also have two special atomic propositions:
- **⊤** (top): Represents a statement that is always true (tautology)
- **⊥** (bottom): Represents a statement that is always false (contradiction)

Think of ⊤ as "1+1=2" and ⊥ as "1+1=3"—statements whose truth values never change.

### Boolean Connectives: The Logical Glue

Just as we use words like "and," "or," and "not" in everyday speech, propositional logic uses precise symbols called **Boolean connectives** to combine atomic propositions:

#### 1. Negation (¬): The "NOT" Operator

**Symbol:** ¬  
**Meaning:** Flips the truth value

**Examples:**
- If A = "It is sunny," then ¬A = "It is not sunny"
- If B = "The door is open," then ¬B = "The door is not open"

**Truth Table:**
| A | ¬A |
|---|-----|
| T | F   |
| F | T   |

#### 2. Conjunction (∧): The "AND" Operator

**Symbol:** ∧  
**Meaning:** True only when both parts are true

**Examples:**
- A ∧ B = "It is sunny AND the door is open"
- "I will go to the movies AND eat popcorn"

**Truth Table:**
| A | B | A ∧ B |
|---|---|-------|
| T | T | T     |
| T | F | F     |
| F | T | F     |
| F | F | F     |

**Real-world analogy:** Like a security system that requires BOTH a keycard AND a fingerprint to open.

#### 3. Disjunction (∨): The "OR" Operator

**Symbol:** ∨  
**Meaning:** True when at least one part is true

**Examples:**
- A ∨ B = "It is sunny OR the door is open"
- "I will have coffee OR tea" (inclusive or—you might have both!)

**Truth Table:**
| A | B | A ∨ B |
|---|---|-------|
| T | T | T     |
| T | F | T     |
| F | T | T     |
| F | F | F     |

#### 4. Implication (→): The "IF...THEN" Operator

**Symbol:** →  
**Meaning:** If the first part is true, then the second must be true

**Examples:**
- A → B = "IF it is raining, THEN the ground is wet"
- "IF you study hard, THEN you will pass the exam"

**Truth Table:**
| A | B | A → B |
|---|---|-------|
| T | T | T     |
| T | F | F     |
| F | T | T     |
| F | F | T     |

**Key insight:** An implication is only false when you have a true antecedent leading to a false consequent—like promising "If it rains, the ground will be wet" but finding dry ground during rain!

#### 5. Equivalence (↔): The "IF AND ONLY IF" Operator

**Symbol:** ↔  
**Meaning:** Both parts have the same truth value

**Examples:**
- A ↔ B = "It is raining IF AND ONLY IF the ground is wet"
- "You pass the course IF AND ONLY IF you score above 70%"

**Truth Table:**
| A | B | A ↔ B |
|---|---|-------|
| T | T | T     |
| T | F | F     |
| F | T | F     |
| F | F | T     |

### Building Complex Formulas

Just like mathematical expressions, we use parentheses to group logical operations and control the order of evaluation:

**Simple Examples:**
- (A ∧ B) → C: "If both A and B are true, then C is true"
- A ∧ (B ∨ C): "A is true, and either B or C (or both) is true"
- ¬(A ∧ B): "It's not the case that both A and B are true"

**Complex Example:**
Let's say:
- A = "It's raining"
- B = "I have an umbrella"  
- C = "I will get wet"

Then: (A ∧ ¬B) → C means "IF it's raining AND I don't have an umbrella, THEN I will get wet"

## Logical Equivalence: When Different Looks the Same

Two formulas are **logically equivalent** if they always have the same truth value, regardless of how we assign truth values to their component propositions. We write this as φ ≡ ψ.

Think of equivalence like saying "six of one, half dozen of the other"—different expressions, same meaning.

### Important Equivalences with Examples

#### De Morgan's Laws (Named after mathematician Augustus De Morgan)

**First Law:** ¬(A ∧ B) ≡ (¬A ∨ ¬B)
- **In words:** "It's not the case that both A and B" is the same as "Either A is false or B is false (or both)"
- **Example:** ¬(sunny ∧ warm) ≡ (¬sunny ∨ ¬warm)
  - "It's not both sunny and warm" = "Either it's not sunny or it's not warm"

**Second Law:** ¬(A ∨ B) ≡ (¬A ∧ ¬B)
- **In words:** "Neither A nor B" is the same as "A is false and B is false"
- **Example:** ¬(coffee ∨ tea) ≡ (¬coffee ∧ ¬tea)
  - "I want neither coffee nor tea" = "I don't want coffee and I don't want tea"

#### Commutative Laws (Order doesn't matter)

**Conjunction:** A ∧ B ≡ B ∧ A
- "Alice is tall and Bob is short" = "Bob is short and Alice is tall"

**Disjunction:** A ∨ B ≡ B ∨ A
- "I'll have pizza or pasta" = "I'll have pasta or pizza"

#### Associative Laws (Grouping doesn't matter)

**Conjunction:** (A ∧ B) ∧ C ≡ A ∧ (B ∧ C)
**Disjunction:** (A ∨ B) ∨ C ≡ A ∨ (B ∨ C)

#### Double Negation
¬¬A ≡ A
- "It's not the case that it's not raining" = "It's raining"

## Rules of Inference: The Tools of Logical Reasoning

Inference rules are like valid chess moves—they tell us how to legally derive new conclusions from existing premises. These nine classical rules form the foundation of all logical reasoning.

### The "Big Three" Essential Rules

#### 1. Modus Ponens (MP): "The Method of Affirming"

**Pattern:**
```
If P then Q
P
-----------
Therefore, Q
```

**Real-world Example:**
```
If it rains, then the ground gets wet
It is raining
---------------------------------
Therefore, the ground gets wet
```

**Why it works:** If we know that P leads to Q, and we observe P happening, then Q must follow. This is perhaps the most intuitive form of reasoning we use daily.

#### 2. Modus Tollens (MT): "The Method of Denying"

**Pattern:**
```
If P then Q
Not Q
-----------
Therefore, Not P
```

**Real-world Example:**
```
If Alice studied hard, then she passed the exam
Alice did not pass the exam
------------------------------------
Therefore, Alice did not study hard
```

**Why it works:** This is reasoning by contradiction. If P would lead to Q, but Q didn't happen, then P couldn't have happened either.

#### 3. Hypothetical Syllogism (HS): "Chain Reasoning"

**Pattern:**
```
If P then Q
If Q then R
-----------
Therefore, If P then R
```

**Real-world Example:**
```
If I study hard, then I get good grades
If I get good grades, then I get into a good college
------------------------------------------------
Therefore, If I study hard, then I get into a good college
```

**Why it works:** This creates logical chains. If A leads to B, and B leads to C, then A must lead to C.

### Additional Powerful Rules

#### 4. Disjunctive Syllogism (DS): "Process of Elimination"

**Pattern:**
```
P or Q
Not P
------
Therefore, Q
```

**Example:**
```
The meeting is either Monday or Tuesday
The meeting is not Monday
--------------------------
Therefore, the meeting is Tuesday
```

#### 5. Constructive Dilemma (CD): "Two-Path Reasoning"

**Pattern:**
```
If P then Q, and If R then S
P or R
-----------------------
Therefore, Q or S
```

**Example:**
```
If it's sunny, we'll go to the beach; If it's rainy, we'll go to the movies
It's either sunny or rainy
--------------------------------------------------------
Therefore, we'll either go to the beach or go to the movies
```

### The "Construction" Rules

#### 6. Conjunction Introduction (Conj): "Combining Facts"

**Pattern:**
```
P
Q
---------
Therefore, P ∧ Q
```

**Example:** If we know "Alice is smart" and "Alice is kind," we can conclude "Alice is smart ∧ kind."

#### 7. Simplification (Simp): "Extracting Facts"

**Pattern:**
```
P and Q
-------
Therefore, P
```

**Example:** From "Alice is smart and kind," we can extract "Alice is smart."

#### 8. Addition (Add): "Expanding Possibilities"

**Pattern:**
```
P
-----------
Therefore, P or Q
```

**Example:** From "It's raining," we can conclude "It's raining or it's sunny" (though this might seem odd, it's logically valid because at least one part of the disjunction is true).

#### 9. Absorption (Abs): "Conditional Strengthening"

**Pattern:**
```
If P then Q
-----------------
Therefore, If P then (P and Q)
```

**Example:** From "If it rains, then I get wet," we can derive "If it rains, then it rains and I get wet."

## Putting It All Together: A Complete Example

Let's work through a practical example using multiple inference rules:

**Given premises:**
1. If Alice studies, then she passes the exam (A → P)
2. If Alice passes the exam, then she graduates (P → G)
3. Alice studies (A)

**Goal:** Prove Alice graduates (G)

**Solution:**
1. A → P (Premise 1)
2. P → G (Premise 2)  
3. A (Premise 3)
4. A → G (From 1, 2 by Hypothetical Syllogism)
5. G (From 3, 4 by Modus Ponens)

This demonstrates how we can chain together multiple inference rules to reach our conclusion, building a bridge from our starting premises to our desired goal.

## Historical Note

These logical principles have an extraordinary pedigree. The inference rules you're learning were first systematized by Aristotle around 350 BCE in his work "Prior Analytics." For over two millennia, these rules have remained the gold standard for valid reasoning, forming the logical foundation for mathematics, computer science, artificial intelligence, and philosophical argumentation.

What you're studying isn't just academic theory—these are the very principles that power search engines, enable computers to make decisions, and help scientists construct rigorous proofs. You're learning the universal language of rational thought itself!
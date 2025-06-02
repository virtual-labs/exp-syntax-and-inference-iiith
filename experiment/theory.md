### Experiment: Syntax and Inference in Propositional Logic

### Introduction
Propositions are sentences that are true or false. Propositional logic makes it possible to formally represent, transform and examine such propositions.

One can distinguish very simple statements (also referred to as atomic) from statements that are made up of other (partial) statements. An <b>atomic</b> proposition is either a propositional variable or the formula <b>&#8868;</b> (pronounced top) or the formula <b>&#8869;</b> (pronounced bottom). They represent a <b>tautology</b> and a <b>contradiction</b> respectively i.e. they are unconditionally true or false. 

#### Boolean Connectives
Boolean connectives such as <b>&#172;</b>, <b>&#8743;</b>, <b>&#8744;</b>, <b>&#8658;</b>, and <b>&#8660;</b> are used to generate complex (non-atomic) sentences. The symbols <b>&#40;</b> and <b>&#41;</b> are used to group sentences to generate increasingly complex sentences.

The process of composing can be repeated any finite number of times to produce a formula. This leads to the inductive definition given [below](#compound-formulas).
It should be noted that this definition is initially interpreted quite strictly. For example, the last two connectors <b>&#8658;</b>, and <b>&#8660;</b> are initially not considered at all. Ultimately, this is not a problem, since we consider them to be shorthand notation for formulas that exclusively use the other connectors, as we will see later.

### Fundamental Concepts

#### Propositional Variables
An atomic proposition is represented by a propositional variable. For propositional variables we use capital letters like A, B, C, ..., using subscripts where appropriate (e.g. A_<sub>1</sub>, A<sub>2</sub>, A<sub>3</sub>, ...). We denote the set of all propositional variables by <b>AV</b>. We assume them to be (countably) infinite.

#### Compound Formulas
Formulas can be composed by using the one-place negation connector <b>&#172;</b>, or by the two-place conjunction connector <b>&#8743;</b>, or by the two-place disjunction connector <b>&#8744;</b>.

#### Equivalence of Formulas
Formulas can be syntactically different, but behave in the same way. Two formulas φ and ψ are equivalent if they take on the same value under every permutation of truth values. If φ and ψ are equivalent, we note this with φ ≡ ψ.

##### Examples of Equivalence:
```
A ∧ B ≡ B ∧ A
A ∧ B ≡ A ∧ (A ∧ B)
A ∧ B ≡ ¬(¬A ∨ ¬B)
```

### Rules of Inference
There are 9 inference rules in classical propositional logic. These are part of a larger set of rules known as <i>Copi's rules</i>.

#### Table of Inference Rules

|   | Inference Rule                | Formulae
|---|-------------------------------|---------------------|
| 1 | Modus Ponens (M.P.)           | p &#8658; q <br/> p <br/> ------- <br/> q        |
| 2 | Modus Tollens (M.T.)          | p &#8658; q<br/> &#172;q <br/> -------<br/> &#172;p    |
| 3 | Hypothetical Syllogism (H.S.) | p &#8658; q <br/> q &#8658; r <br/> ------- <br/> p &#8658; r |
| 4 | Disjunctive Syllogism (D.S.)  | p &#8744; q <br/> &#172;p <br/>------- <br/> q       |
| 5 | Constructive Dilemma (C.D.)  |(p &#8658; q).(r &#8658; s) <br/> p &#8744; r <br/>---------------- <br/> q &#8744; s                    |
| 6 | Absorption (Abs.)             | p &#8658; q <br/>-------------<br/>p &#8658; (p &#8743; q)                   |
| 7 | Simplification (Simp.)        | p &#8743; q <br/>-------<br/>p                    |
| 8 | Conjunction (Conj.)           | p<br/>q<br/>-------<br/>p &#8743; q                    |
| 9 | Addition (Add.)               | p<br/>-------<br/>p &#8744; q                    |
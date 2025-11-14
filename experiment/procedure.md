## Overview
This experiment introduces you to the fascinating world of formal logic through an interactive proof assistant. You'll learn to construct valid logical arguments step-by-step, just like mathematicians have done for centuries!
---

## Phase 1: Pre-Experiment Preparation

### 1.1 Knowledge Foundation
Before beginning the interactive simulation, ensure you understand these fundamental concepts:

**Logical Connectives** (The building blocks of logic):
- **¬** (Negation): "NOT" - reverses the truth value
- **∧** (Conjunction): "AND" - true only when both parts are true  
- **∨** (Disjunction): "OR" - true when at least one part is true
- **→** (Implication): "IF...THEN" - the foundation of logical reasoning
- **↔** (Equivalence): "IF AND ONLY IF" - true when both sides have the same truth value
- **⊥** (Contradiction): represents a false statement

**Essential Inference Rules**:
- **Modus Ponens (MP)**: From "If P then Q" and "P", conclude "Q"
- **Modus Tollens (MT)**: From "If P then Q" and "not Q", conclude "not P"  
- **Hypothetical Syllogism (HS)**: From "If P then Q" and "If Q then R", conclude "If P then R"
- **Conjunction Introduction**: From "P" and "Q", conclude "P and Q"
- **Conjunction Elimination**: From "P and Q", conclude "P" (or "Q")
- **Disjunctive Syllogism**: From "P or Q" and "not P", conclude "Q"

### 1.2 Assessment Preparation
Complete the pretest to establish your baseline understanding of logical reasoning concepts.

---

## Phase 2: Interactive Proof Construction

### 2.1 System Familiarization
When you first access the simulation interface, you'll encounter:

**Main Interface Components**:
1. **Goal Panel** (left): Shows the formula you need to prove
2. **Derivation Sequence** (main area): Your step-by-step proof construction
3. **Floating Action Buttons**: Quick access to rules and instructions
4. **Control Buttons**: Tools for managing your proof

**Pro Tip**: The interface is designed to mirror how professional logicians work - with premises, inference rules, and systematic derivation!

### 2.2 Starting Your First Proof

#### Step 1: Generate a New Problem
- Click the **"New Problem"** button to receive a random logical challenge
- The system will present you with:
  - **Premises**: Initial statements you can use (shown with blue "Premise" badges)
  - **Goal**: The target formula you must derive (displayed prominently in the Goal panel)

#### Step 2: Analyze the Problem Structure
- **Read the goal carefully**: What are you trying to prove?
- **Examine the premises**: What logical statements do you have to work with?
- **Identify potential inference paths**: Which rules might help you progress from premises to goal?

### 2.3 Constructing Your Proof

#### Step 3: Select Relevant Statements
- **Click on statements** in the derivation sequence to select them
- Selected statements will be highlighted with a blue border
- **Order matters**: For some rules like Modus Ponens, the sequence of selection affects the result
- You can select multiple statements as required by different inference rules

**Important**: Some rules require exactly 2 premises, others require only 1. Pay attention to the rule requirements!

#### Step 4: Choose an Inference Rule
- Click the **Rules button** (document icon) to open the inference rules panel
- Browse through available rules and their descriptions
- **Click on a rule** to select it - selected rules will be highlighted
- Each rule shows:
  - **Name**: The formal name of the inference rule
  - **Pattern**: What type of statements it works with
  - **Description**: Plain English explanation of what the rule does

#### Step 5: Apply the Rule
- Once you have selected both statements and a rule, click **"Apply Rule"**
- The system will:
  - Validate that your selection matches the rule requirements
  - Automatically derive the conclusion if valid
  - Add the new statement to your derivation sequence
  - Show the justification (which rule was used and which statements)

**Success Indicator**: Valid applications will add new statements marked as "Inferred" with the rule name and line references.

### 2.4 Advanced Proof Techniques

#### Systematic Approach
1. **Work backwards**: Start from the goal and think about what rules could produce it
2. **Work forwards**: See what new statements you can derive from your current premises
3. **Look for patterns**: Common proof structures often repeat across problems

#### Using Control Features
- **"Clear"**: Deselect all currently selected statements and rules
- **"Reset"**: Return to just the original premises (useful if you get stuck)
- **"Hint"**: Receive guidance on potential next steps (available for some problems)
- **"Validate"**: Check if you've successfully derived the goal

---

## Phase 3: Mastery and Assessment

### 3.1 Proof Validation
When you believe you've completed a proof:
1. Click **"Validate"** to check your work
2. **Success**: Green message confirms you've derived the goal
3. **Incomplete**: Red message indicates the goal hasn't been reached yet

### 3.2 Problem Progression
- Try multiple problems to practice different inference patterns
- Each problem may require different combinations of rules
- **Challenge yourself**: Attempt to solve problems using the minimum number of steps

### 3.3 Common Patterns to Master
1. **Chain of Implications**: Using Hypothetical Syllogism to connect multiple "if-then" statements
2. **Contradiction Resolution**: Using Modus Tollens when you have negative information
3. **Conjunction Handling**: Breaking apart "and" statements to use individual components
4. **Disjunctive Cases**: Working with "or" statements to eliminate possibilities

---

## Phase 4: Skill Consolidation

### 4.1 Self-Assessment
After completing several proofs successfully:
- Can you identify which inference rule to use just by looking at the statements?
- Are you comfortable with the logical symbols and their meanings?
- Can you construct proofs efficiently without excessive backtracking?

### 4.2 Final Assessment
Complete the posttest to measure your improvement in:
- Understanding of logical connectives
- Application of inference rules
- Construction of valid arguments
- Recognition of logical patterns

---

## Troubleshooting and Tips

### Common Issues and Solutions

**"Invalid Rule Application"**:
- Check that you've selected the correct number of statements
- Verify that the statements match the rule's pattern requirements
- Remember that order of selection matters for some rules

**Getting Stuck on a Proof**:
- Use the "Hint" button if available
- Try working backwards from the goal
- Consider what rules could produce the type of statement you need
- Use "Reset" to start fresh with just the premises

**Understanding Symbol Meanings**:
- Refer to the Info panel (information icon) for symbol reference
- Practice reading formulas aloud using natural language
- Remember: → means "if...then", ∧ means "and", ∨ means "or"

### Maximizing Learning

1. **Don't rush**: Take time to understand why each step is valid
2. **Experiment**: Try different approaches to the same problem
3. **Pattern recognition**: Notice how similar logical structures appear across problems
4. **Verbalize**: Try explaining your reasoning out loud or in writing

**Achievement Goal**: By the end of this experiment, you should be able to construct formal logical proofs confidently and understand the rigorous reasoning that underlies mathematical and scientific arguments!

---

## Fun Facts About Logic

- **Historical Note**: The inference rules you're using were systematized by Aristotle around 350 BCE
- **Modern Applications**: These same logical principles power search engines, AI systems, and computer programming
- **Universal Language**: Logical notation looks the same whether you're in New York, Tokyo, or Mumbai - it's truly universal!
- **Precision Power**: Formal logic eliminates ambiguity that plagues natural language - every statement has a definite meaning
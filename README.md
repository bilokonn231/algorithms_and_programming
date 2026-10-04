# Types of Algorithms

An **algorithm** is a finite sequence of unambiguous instructions executed to solve a problem or perform a computation. 

Algorithms are categorized primarily by their control flow—how instructions are structured and executed relative to dynamic conditions.

---

## 1. Linear Algorithms

A **linear algorithm** executes instructions in a fixed, strictly sequential order from start to finish. It contains no decision points, jump statements, or alternative execution paths.

### Characteristics
* **Execution Flow:** Sequential ($1 \rightarrow 2 \rightarrow 3$).
* **Determinism:** Executes the exact same sequence of steps for every input.
* **Complexity:** $O(1)$ structural complexity (no branching logic).

### Control Flow Diagram
```text
[Start]
   │
   ▼
[Instruction 1]
   │
   ▼
[Instruction 2]
   │
   ▼
[Instruction 3]
   │
   ▼
[Output Result]
   │
   ▼
[End]
```

### Example: Rectangle Area Calculation

#### Pseudocode
```pascal
BEGIN
    Input length
    Input width
    area <- length * width
    Output area
END
```

---

## 2. Branched (Conditional) Algorithms

A **branched algorithm** evaluates one or more conditional expressions to determine which branch of execution to follow. 

### Characteristics
* **Execution Flow:** Dynamic and non-linear; depends on state evaluation.
* **Flexibility:** Adapts operations based on variable inputs or runtime states.
* **Constructs:** Implemented via conditional statements (`IF-THEN-ELSE`, `SWITCH-CASE`).

### Control Flow Diagram
```text
         [Start]
            │
            ▼
     /  Condition?  \
    /                \
  (True)           (False)
    │                 │
    ▼                 ▼
[Branch A]        [Branch B]
    │                 │
    └────────┬────────┘
             │
             ▼
       [Output Result]
             │
             ▼
           [End]
```

### Example: Sign Determination

#### Pseudocode
```pascal
BEGIN
    Input number
    IF number >= 0 THEN
        Output "Positive or Zero"
    ELSE
        Output "Negative"
    END IF
END
```

---

## 3. Structural Comparison

| Feature | Linear Algorithm | Branched Algorithm |
| :--- | :--- | :--- |
| **Execution Order** | Strictly sequential | Conditional / Non-linear |
| **Alternative Paths** | None ($1$ path) | Multiple ($\ge 2$ paths) |
| **Control Structures** | Sequential statements | `IF`, `THEN`, `ELSE`, `SWITCH` |
| **Path Complexity** | Constant | Variable based on conditions |
| **Primary Use Case** | Fixed calculations, formulas | Validation, decision logic |

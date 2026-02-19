# Algorithm and Flowchart Workshop – Muthana Fouad

# Workshop: Algorithm and Flowchart

For each question in this workshop, you must complete **two** things:

1.  **Write the pseudocode**
2.  **Draw the flowchart** using either
    - **Option 1:** Draw.io (recommended) → export image → upload to
      your repository → link it in this file
    - **Option 2 (optional):** Write a Mermaid flowchart directly in
      Markdown
    - **Option 3 (optional):** Any other valid method

👉 **IMPORTANT:** At the **bottom of each question**, add the
following sections:

### ✔ Pseudocode

### ✔ Flowchart

---

## 1. Check Even or Odd Number

Design an algorithm and flowchart that take a number as input and
determine whether it is even or odd.

### ✔ Pseudocode

```text
START
    INPUT number
    IF number % 2 == 0 THEN
        PRINT Even
    ELSE
        PRINT Odd
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> I[/Get input N/]
    I --> B{N % 2 == 0 ?}
    B -->|Yes| C[/Print Even/]
    B -->|No| D[/Print Odd/]
    C --> E([End])
    D --> E([End])
```

---

## 2. Calculate Total and Average Marks

Write the algorithm and draw the flowchart for a program that inputs
marks for 3 subjects, calculates the total and average, and displays
both.

---

### ✔ Pseudocode

```text
START
    INPUT mark1
    INPUT mark2
    INPUT mark3
    total = mark1 + mark2 + mark3
    average = total / 3
    PRINT total
    PRINT average
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input mark1/]
    B --> C[/Input mark2/]
    C --> D[/Input mark3/]
    D --> E[total = mark1 + mark2 + mark3]
    E --> F[average = total / 3]
    F --> G[/Print total/]
    G --> H[/Print average/]
    H --> I([End])
```

---

## 3. Display Multiplication Table

Create an algorithm and flowchart that input a number and display its
multiplication table from 1 to 10 using a loop.

---

### ✔ Pseudocode

```text
START
    INPUT N
    FOR i = 1 TO 10 DO
        result = N * i
        PRINT N x i = result
    END FOR
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input N/]
    B --> C[Set i = 1]
    C --> D{i <= 10?}
    D -->|Yes| E[result = N * i]
    E --> F[/Print N x i = result/]
    F --> G[i = i + 1]
    G --> D
    D -->|No| H([End])
```

---

## 4. Positive, Negative, or Zero Check

Write the algorithm and flowchart to input a number and display whether
it is positive, negative, or zero.

---

### ✔ Pseudocode

```text
START
    INPUT number
    IF number > 0 THEN
        PRINT Positive
    ELSE IF number < 0 THEN
        PRINT Negative
    ELSE
        PRINT Zero
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input number/]
    B --> C{number > 0?}
    C -->|Yes| D[/Print Positive/]
    C -->|No| E{number < 0?}
    E -->|Yes| F[/Print Negative/]
    E -->|No| G[/Print Zero/]
    D --> H([End])
    F --> H
    G --> H
```

---

## 5. Simple Interest Calculator

Create an algorithm and flowchart for a program that calculates simple
interest using the formula:

**SI = (P × R × T) / 100**

- **P = Principal** → original amount of money
- **R = Rate of Interest** → percentage per year
- **T = Time** → number of years

---

### ✔ Pseudocode

```text
START
    INPUT P
    INPUT R
    INPUT T
    SI = (P * R * T) / 100
    PRINT SI
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input P/]
    B --> C[/Input R/]
    C --> D[/Input T/]
    D --> E[SI = P * R * T / 100]
    E --> F[/Print SI/]
    F --> G([End])
```

---

## 6. Average Temperature Calculation

Write the algorithm and draw the flowchart for a program that takes the
temperature of 7 days, finds the average temperature, and displays it.

---

### ✔ Pseudocode

```text
START
    total = 0
    FOR day = 1 TO 7 DO
        INPUT temp
        total = total + temp
    END FOR
    average = total / 7
    PRINT average
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Set total = 0]
    B --> C[Set day = 1]
    C --> D{day <= 7?}
    D -->|Yes| E[/Input temp/]
    E --> F[total = total + temp]
    F --> G[day = day + 1]
    G --> D
    D -->|No| H[average = total / 7]
    H --> I[/Print average/]
    I --> J([End])
```

---

## 7. Calculate Area of a Rectangle

Create an algorithm and flowchart to input length and width, calculate
the area (**Area = Length × Width**), and display the result.

---

### ✔ Pseudocode

```text
START
    INPUT length
    INPUT width
    area = length * width
    PRINT area
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input length/]
    B --> C[/Input width/]
    C --> D[area = length * width]
    D --> E[/Print area/]
    E --> F([End])
```

---

## 8. Determine Pass or Fail

Write the algorithm and draw the flowchart for a program that takes a
student's average marks and displays **"Pass"** if average ≥ 50,
otherwise **"Fail"**.

---

### ✔ Pseudocode

```text
START
    INPUT average
    IF average >= 50 THEN
        PRINT Pass
    ELSE
        PRINT Fail
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input average/]
    B --> C{average >= 50?}
    C -->|Yes| D[/Print Pass/]
    C -->|No| E[/Print Fail/]
    D --> F([End])
    E --> F
```

---

## 9. Calculate Factorial of a Number

Write the algorithm and draw the flowchart that input a number and
calculate its factorial using a loop.

---

### ✔ Pseudocode

```text
START
    INPUT N
    factorial = 1
    FOR i = 1 TO N DO
        factorial = factorial * i
    END FOR
    PRINT factorial
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input N/]
    B --> C[Set factorial = 1]
    C --> D[Set i = 1]
    D --> E{i <= N?}
    E -->|Yes| F[factorial = factorial * i]
    F --> G[i = i + 1]
    G --> E
    E -->|No| H[/Print factorial/]
    H --> I([End])
```

---

## 10. Calculate Discount on Purchase

Write the algorithm and draw the flowchart for a program that inputs the
purchase amount and gives a **10% discount** if the amount is greater
than 1000.

---

### ✔ Pseudocode

```text
START
    INPUT amount
    IF amount > 1000 THEN
        discount = amount * 0.10
    ELSE
        discount = 0
    ENDIF
    finalAmount = amount - discount
    PRINT discount
    PRINT finalAmount
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input amount/]
    B --> C{amount > 1000?}
    C -->|Yes| D[discount = amount * 0.10]
    C -->|No| E[discount = 0]
    D --> F[finalAmount = amount - discount]
    E --> F
    F --> G[/Print discount/]
    G --> H[/Print finalAmount/]
    H --> I([End])
```

---

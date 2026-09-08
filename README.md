# FACTORIAL-OF-A-NUMBER
# FACTORIAL OF A NUMBER USING 8051 (Keil)

## AIM
To write and execute an Assembly language program to perform the factorial of a number using 8051 Keil.

---

## APPARATUS REQUIRED
- Personal computer with Keil software

---

## ALGORITHM
1. **Start**
2. **Input**: Read the number `n`.
3. **Initialize**:
   - Set factorial to `1`.
   - Set `i` to `1`.
4. **Loop**: While `i` is less than or equal to `n`:
   - Multiply factorial by `i`.
   - Increment `i` by `1`.
5. **Output**: Store or print the value of factorial.
6. **End**

---

## FLOWCHART
<img width="506" height="525" alt="image" src="https://github.com/user-attachments/assets/f3b47187-6f0f-490c-8704-f2973cb2b276" />


---

## PROGRAM
```asm
ORG 0000H
MOV R0, #30H     ; R0 points to memory location 30H
MOV A, @R0       ; Load number into A
MOV R1, A        ; Copy number to R1 (counter)
MOV A, #01H      ; A = 1 (initial factorial result)
FACT:
MOV B, R1        ; Move counter to B
MUL AB           ; A = A × B
DJNZ R1, FACT    ; Decrement R1 and repeat until zero
MOV 31H, A       ; Store result in 31H
END

```
OUTPUT

<img width="739" height="408" alt="image" src="https://github.com/user-attachments/assets/8decfdcc-b9b2-46e9-a341-6dc803082c9e" />


---
MANUAL CALCULATIONS


<img width="471" height="372" alt="WhatsApp Image 2026-05-22 at 7 43 36 AM" src="https://github.com/user-attachments/assets/046989c1-def7-456c-9207-4bb0bcbb2698" />



---

RESULT

Thus, the factorial of a number was calculated and executed successfully using 8051 Keil.

---



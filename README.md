# Sorting of numbers in a sequence
## Exp 3 (a) : Ascending Order
## Aim :
To write and execute an 8085 program to sort a set of numbers in ascending order.
## Apparatus Required:
•	8085 Online Simulator (8085simulator.github.io or similar)
<br>•	Test input data
<br>•	Instruction set reference
## Algorithm (Ascending Order):
1.	Load count from memory into register C.
2.	Subtract 1 from count and store in B (outer loop counter).
3.	Outer loop (B times):
<br>Point HL to the first data.
<br>Copy C to D (inner loop counter).
<br>Inner loop (D times):
<br>Compare adjacent elements.
<br>If current > next, swap them.
<br>Decrement B and repeat.
4.	End.
## Program:

; Input : 2 numbers at 8050H and 8051H
; Output: Sorted in same locations
LXI H,8050H   ; HL -> first number
MOV A,M       ; A = first
INX H         ; HL -> second
CMP M         ; Compare A with second
JC END        ; If first < second → already sorted
; Swap
MOV D,M       ; D = second
MOV M,A       ; Put first into [8051H]
DCX H         ; Back to first
MOV M,D       ; Put second into [8050H]
END: HLT

## Output: 

![WhatsApp Image 2025-09-10 at 09 44 07_6b99140f](https://github.com/user-attachments/assets/25ffdf11-0d71-45cd-9353-49eb44902b82)

## Result:
The 8085 assembly language program was successfully executed to sort a set of numbers in ascending order.

## Exp 3 (b) : Descending Order
## Aim:
To write and execute an 8085 program to sort a set of numbers in descending order.
## Apparatus Required:
•	8085 Online Simulator
•	Hex input data
•	Instruction set reference
## Algorithm (Descending Order):
1.	Load the count of numbers from memory into register C.
2.	Subtract 1 from count and store in B.
3.	Outer loop (B times):
<br>Point HL to first number.
<br>Copy count to D.
<br>Inner loop (D times):
<br>Compare adjacent numbers.
<br>If current < next, swap them.
4. Repeat until sorted.
## Program:

; Input : 2 numbers at 8050H and 8051H
; Output: Sorted (descending) in same locations
LXI H,8050H   ; HL -> first number
MOV A,M       ; A = first
INX H         ; HL -> second
CMP M         ; Compare A with second
JNC END       ; If A >= second → already descending
; Swap
MOV D,M       ; D = second
MOV M,A       ; Put first into [8051H]
DCX H         ; Back to first
MOV M,D       ; Put second into [8050H]
END: HLT


## Output: 

![WhatsApp Image 2025-09-10 at 09 44 06_39efc31f](https://github.com/user-attachments/assets/451da1f9-d22d-4197-9dee-5c0e0dd45783)


## Result:
The 8085 assembly language program was successfully executed to sort a set of numbers in descending order.

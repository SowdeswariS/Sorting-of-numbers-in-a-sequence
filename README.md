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
## Output: 
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
## Output: 
## Result:
The 8085 assembly language program was successfully executed to sort a set of numbers in descending order.

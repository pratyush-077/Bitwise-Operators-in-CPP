# Bitwise operators in C++
# Pratyush Saha
# PRN-24070123078
Bitwise operators work directly on the binary representation (bits) of integers.
They allow you to manipulate bits for low-level programming, performance optimization, and hardware control.

Types of Bitwise Operators & Their Functions
Operator	Name	Function (What it does)	Example (a = 5, b = 3)
&	Bitwise AND	Compares each bit; returns 1 if both bits are 1, else 0	a & b = 1 (0101 & 0011 = 0001)
`	`	Bitwise OR	Compares each bit; returns 1 if at least one bit is 1
^	Bitwise XOR	Returns 1 if bits are different, else 0	a ^ b = 6 (0101 ^ 0011 = 0110)
~	Bitwise NOT	Inverts all bits (1 becomes 0, 0 becomes 1). Also changes sign (two’s complement).	~a = -6 (if a = 5)
<<	Left Shift	Shifts bits to the left (adds zeros at right). Multiplies by 2 per shift.	a << 1 = 10 (0101 → 1010)
>>	Right Shift	Shifts bits to the right (drops bits on right). Divides by 2 per shift.	a >> 1 = 2 (0101 → 0010)

Binary Example (Step by Step)
For a = 5 and b = 3:

a in binary: 0101

b in binary: 0011

AND (&) → 0101 & 0011 = 0001 (1)

OR (|) → 0101 | 0011 = 0111 (7)

XOR (^) → 0101 ^ 0011 = 0110 (6)

NOT (~a) → Invert 0101 → 1010 (two’s complement = -6)

Left Shift (a << 1) → 0101 → 1010 (10)

Right Shift (a >> 1) → 0101 → 0010 (2)

Where Are Bitwise Operators Used?

Embedded systems & low-level programming (hardware control).

Data compression & encryption (XOR is common in cryptography).

Performance optimization (multiplication/division by powers of 2 using shifts).

Masking operations (turning specific bits ON/OFF).


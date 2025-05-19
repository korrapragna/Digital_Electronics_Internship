# DIGITAL ELECTRONICS

# Table of Contents

- [What is Digital Electronics](#What-is-Digital-Electronics)

- [Applications of Digital Electronics](#Applications-of-Digital-Electronics).

- [Digital vs Analog Signals](#Digital-vs-Analog-Signals)

- [Number System](#Number-System)

- [Conversion between Number System](#Conversion-between-Number-System)

- [Basic Logic gates](#Basic-Logic-gates)

- [Integrated Circuits Ic's](#Integrated-Circuits-Ic's)

# What is Digital Electronics
Digital electronics is a branch of electronics that deals with systems that use discrete (distinct) signal levels, typically represented by binary numbers — 0 and 1. Unlike analog electronics, where signals can vary smoothly across a range of values, digital electronics processes information using only two states (usually referred to as LOW and HIGH, or OFF and ON).

0 → low voltage

1 → high voltage
# Applications of Digital Electronics
1.Computing

2.Communication

3.Entertainment

4.Transportation

5.Industrial control

6.Medical equipment

7.Military

8.Home appliances

9.Environmental monitoring

10.Security
# Digital vs Analog Signals
| Feature            | **Analog Signal**                          | **Digital Signal**                           |
| ------------------ | ------------------------------------------ | -------------------------------------------- |
| **Nature**         | Continuous signal                          | Discrete signal (binary: 0s and 1s)          |
| **Representation** | Varies smoothly over time                  | Represented in steps or levels               |
| **Examples**       | Human voice, analog clock, radio waves     | Computers, digital clocks, digital phones    |
| **Precision**      | Less precise, can degrade with noise       | More precise and resilient to noise          |
| **Signal Form**    | Sine waves                                 | Square waves                                 |
| **Storage**        | Difficult and often lossy                  | Easy and lossless                            |
| **Transmission**   | Can lose quality over long distances       | Maintains quality over long distances        |
| **Hardware**       | Requires amplifiers, more complex circuits | Requires encoders/decoders, simpler circuits |
| **Bandwidth**      | Typically lower                            | Typically higher                             |
# Logic Levels
Logic levels refer to specific voltage ranges used in digital circuits to represent binary states: 0 (LOW) and 1 (HIGH).
| **Logic Family**                                   | **Logic 0 (LOW)**  | **Logic 1 (HIGH)** | **Supply Voltage (Vcc)** |
| -------------------------------------------------- | ------------------ | ------------------ | ------------------------ |
| **TTL (Transistor-Transistor Logic)**              | 0 V to 0.8 V       | 2.0 V to 5.0 V     | 5 V                      |
| **CMOS (Complementary Metal-Oxide-Semiconductor)** | 0 V to \~1/3 Vcc   | \~2/3 Vcc to Vcc   | 3.3 V, 5 V, etc.         |
| **LVTTL (Low Voltage TTL)**                        | 0 V to 0.8 V       | 2.0 V to 3.3 V     | 3.3 V                    |
| **LVCMOS (Low Voltage CMOS)**                      | \~0 V to 0.3 × Vcc | \~0.7 × Vcc to Vcc | 1.8 V, 2.5 V, 3.3 V      |
# Number System
A number system is a way to represent and express numbers using a set of symbols or digits. In digital electronics, number systems are used to represent data and perform calculations inside digital circuits and computers.
# Different Number Systems are BINARY, OCTAL,DECIMAL, HEXADECIMAL
| **Number System** | **Base** | **Digits Used**               | **Example** | **Used In**                                |
| ----------------- | -------- | ----------------------------- | ----------- | ------------------------------------------ |
| **Binary**        | 2        | 0, 1                          | 1011₂       | Computers, digital electronics             |
| **Octal**         | 8        | 0 to 7                        | 17₈         | Shorter binary representation              |
| **Decimal**       | 10       | 0 to 9                        | 345₁₀       | Everyday arithmetic, human counting system |
| **Hexadecimal**   | 16       | 0 to 9 and A to F (A=10…F=15) | 2F₁₆        | Programming, memory addresses, colors      |
# Conversion between Number System

# 1. Binary → Decimal
   
Binary: 1011₂

= (1×2³) + (0×2²) + (1×2¹) + (1×2⁰)

= 8 + 0 + 2 + 1

= 11₁₀

# 2. Decimal → Binary
Decimal: 13₁₀

13 ÷ 2 = 6 remainder 1

6 ÷ 2 = 3 remainder 0

3 ÷ 2 = 1 remainder 1

1 ÷ 2 = 0 remainder 1

Read remainders bottom to top → 1101₂

# 3. Binary → Octal
Binary: 110110₂

Group in 3 bits → 110 | 110

110₂ = 6₈

110₂ = 6₈

Result → 66₈

# 4. Octal → Binary
Octal: 57₈

5₈ → 101₂

7₈ → 111₂

Result → 101111₂

# 5. Binary → Hexadecimal
Binary: 10101110₂

Group in 4 bits → 1010 | 1110

1010₂ = A₁₆

1110₂ = E₁₆

Result → AE₁₆

# 6. Hexadecimal → Binary
Hex: 3F₁₆

3₁₆ → 0011₂

F₁₆ → 1111₂

Result → 00111111₂

# 7. Decimal → Octal
Decimal: 125₁₀

125 ÷ 8 = 15 remainder 5

15 ÷ 8 = 1 remainder 7

1 ÷ 8 = 0 remainder 1

Read remainders bottom to top → 175₈

# 8. Octal → Decimal
Octal: 745₈

= (7×8²) + (4×8¹) + (5×8⁰)

= (7×64) + (4×8) + (5×1)

= 448 + 32 + 5

= 485₁₀

# 9. Decimal → Hexadecimal
Decimal: 254₁₀

254 ÷ 16 = 15 remainder 14 (E)

15 ÷ 16 = 0 remainder 15 (F)

Read remainders bottom to top → FE₁₆

# 10. Hexadecimal → Decimal
Hex: 2A₁₆

= (2×16¹) + (A×16⁰)

= (2×16) + (10×1)

= 32 + 10

= 42₁₀

# 11. Octal → Hexadecimal
Octal: 745₈

Step 1: Octal → Binary

7 → 111

4 → 100

5 → 101

Binary = 111100101₂

Step 2: Binary → Hex

Group 4 bits: 0011 | 1100 | 101 (pad left 0 → 0101)

0011 → 3

1100 → C

0101 → 5

Result → 3C5₁₆

# 12. Hexadecimal → Octal
Hex: 2F₁₆

Step 1: Hex → Binary

2 → 0010

F → 1111

Binary = 00101111₂

Step 2: Binary → Octal

Group 3 bits: 000 | 101 | 111

000 → 0

101 → 5

111 → 7

Result → 057₈

# Basic Logic gates 
# 1.AND GATE
# Symbol :
The standard symbol for a 2-input AND gate looks like this:

![image](https://github.com/user-attachments/assets/3db401a1-1c50-4a3a-a56b-0b6e209aba5f)

# Function :
The AND gate performs a logical multiplication. It outputs HIGH (1) only if all inputs are HIGH (1). For two inputs A and B, the output Q is given by:

Q=A⋅B
Or in Boolean algebra:

𝐴
∧
𝐵

Q=A∧B
# Truth table :
| INP A |INP B | OUTPUT Y    |
| -     | -    | ----------- |
| 0     | 0    | 0           |
| 0     | 1    | 0           |
| 1     | 0    | 0           |
| 1     | 1    | 1           |
# 2.OR GATE
# Symbol :
Standard symbol for a 2-input OR gate:

![image](https://github.com/user-attachments/assets/5ddd0cbf-eb58-4782-887d-3dcf2427bf18)

# Function :
The OR gate performs logical addition. It outputs HIGH (1) if at least one of its inputs is HIGH. For two inputs A and B, the output Q is:

Q=A+B
Or in Boolean logic:

Q=A∨B
# Truth table :
|INP A |INP B | OUTPUT Y |
| -    | -    | ---------- |
| 0    | 0    | 0          |
| 0    | 1    | 1          |
| 1    | 0    | 1          |
| 1    | 1    | 1          |
# 3.NOT GATE 
# Symbol:
Standard symbol for a NOT gate:

![image](https://github.com/user-attachments/assets/39234de8-5b97-4111-afbb-c48b097546ec)

# Function :
The NOT gate inverts its input:

If the input is 1, the output is 0.

If the input is 0, the output is 1.

In Boolean logic:

Q= 
A
 
or

Q=¬A
# Truth table :
| INP A | OUTPUT Y  |
| -     | --------- |
| 0     | 1         |
| 1     | 0         |
# 4.NAND GATE
# Symbol :
It's similar to the AND gate symbol but with a small circle (representing NOT) at the output.

![image](https://github.com/user-attachments/assets/deaf3611-c7ad-4437-8c91-56166d9c4226)

# Function :

The NAND (Not AND) gate outputs:

0 only when both inputs are 1

Otherwise, it outputs 1

Output= 
A⋅B
# Truth table :
|INP A |INP B |(A.B)        | OUTPUT Y                  |
| -    | -    | ----------- | ------------------------- |
| 0    | 0    | 0           | 1                         |
| 0    | 1    | 0           | 1                         |
| 1    | 0    | 0           | 1                         |
| 1    | 1    | 1           | 0                         |
# 5.NOR GATE
# Symbol :
![image](https://github.com/user-attachments/assets/627f332b-e977-42de-9886-a492488e4d49)

# Function :

A NOR (Not OR) gate gives an output of 1 only when both inputs are 0.

It is the inverse of the OR gate.
# Truth Table :
|INP A | INP B | OUTPUT Y |
| -    | -     | ------- |
| 0    | 0     | 1       |
| 0    | 1     | 0       |
| 1    | 0     | 0       |
| 1    | 1     | 0       |
# 6.XOR GATE
# Symbol :

![image](https://github.com/user-attachments/assets/d9f9f1df-f2ad-4fe1-91de-bd90ceb47b5f)

# Function :
The XOR (Exclusive OR) gate gives an output of 1 only when the inputs are different.

Boolean Expression : Y = A ⊕ B = A̅·B + A·B̅

# Truth table :
|INP A |INP B | OUTPUT Y |
| -    | -    | ------- |
| 0    | 0    | 0       |
| 0    | 1    | 1       |
| 1    | 0    | 1       |
| 1    | 1    | 0       |

# 7.XNOR GATE :
# Symbol :

![image](https://github.com/user-attachments/assets/7f54ebf7-8a5a-48de-897e-bc60afc44ba0)

# Function :
The XNOR (Exclusive NOR) gate gives an output of 1 only when the inputs are the same.

Boolean Expression : Y = (A ⊕ B)̅ = A·B + A̅·B̅

# Truth table :
| INP A |INP B | OUTPUT Y |
| -     | - | -------- |
| 0     | 0 | 1        |
| 0     | 1 | 0        |
| 1     | 0 | 0        |
| 1     | 1 | 1        |

# Integrated Circuits Ic's








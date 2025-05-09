# What is digital electronics?
Digital electronics is a branch of electronics that deals with systems that use discrete (distinct) signal levels, typically represented by binary numbers — 0 and 1. Unlike analog electronics, where signals can vary smoothly across a range of values, digital electronics processes information using only two states (usually referred to as LOW and HIGH, or OFF and ON).

0 → low voltage

1 → high voltage
# Applications of DE
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
# Conversion between number system

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

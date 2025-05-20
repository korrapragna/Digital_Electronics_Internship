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
what is an Ic?
An IC (Integrated Circuit) is a small electronic device made of a semiconductor material (usually silicon) that contains a large number of tiny components like:

- Transistors

- Resistors

- Capacitors

- Diodes

Here is a tabular summary of common logic gates, their corresponding IC numbers, descriptions, number of gates per IC, and pin configuration:

| Logic Gate | IC Number (TTL Series) | Description                     | No. of Gates in IC | Pin Count |
| ---------- | ---------------------- | ------------------------------- | ------------------ | --------- |
| AND        | 7408                   | Quad 2-input AND gate           | 4                  | 14        |
| OR         | 7432                   | Quad 2-input OR gate            | 4                  | 14        |
| NOT        | 7404                   | Hex inverter (NOT gate)         | 6                  | 14        |
| NAND       | 7400                   | Quad 2-input NAND gate          | 4                  | 14        |
| NOR        | 7402                   | Quad 2-input NOR gate           | 4                  | 14        |
| XOR        | 7486                   | Quad 2-input Exclusive-OR gate  | 4                  | 14        |
| XNOR       | 74266 or 74LS266       | Quad 2-input Exclusive-NOR gate | 4                  | 14        |

# 1. 7408-Quad 2-input AND gate

# Pin Diagram:

![image](https://github.com/user-attachments/assets/a79dcd24-17f3-40aa-b717-ca9ff0577392)


![image](https://github.com/user-attachments/assets/75d51c86-38e3-43ba-a62d-6abf5674be80)

https://www.tinkercad.com/things/eDdC36KJHwt-7408-quad-2-input-and-gate?sharecode=QM7E7AOvY_HAbfIPHpO0O6tC0lS-r3uNRAtc4ZyuGdY

# Pin Description
| **Pin No.** | **Name** | **Function**                 |
| ----------- | -------- | ---------------------------- |
| 1           | 1A       | Input A for Gate 1           |
| 2           | 1B       | Input B for Gate 1           |
| 3           | 1Y       | Output of Gate 1 (1A AND 1B) |
| 4           | 2A       | Input A for Gate 2           |
| 5           | 2B       | Input B for Gate 2           |
| 6           | 2Y       | Output of Gate 2 (2A AND 2B) |
| 7           | GND      | Ground (0V)                  |
| 8           | 3Y       | Output of Gate 3 (3A AND 3B) |
| 9           | 3A       | Input A for Gate 3           |
| 10          | 3B       | Input B for Gate 3           |
| 11          | 4Y       | Output of Gate 4 (4A AND 4B) |
| 12          | 4A       | Input A for Gate 4           |
| 13          | 4B       | Input B for Gate 4           |
| 14          | Vcc      | Power Supply (+5V typical)   |

- Each AND gate outputs HIGH only if both inputs are HIGH.

- Power: Pin 14 (Vcc), Ground: Pin 7.

# 2. 7432-Quad 2-input OR gate

# Pin Diagram:

![image](https://github.com/user-attachments/assets/79427904-2eb1-4733-86b8-12075cac05fb)


![image](https://github.com/user-attachments/assets/dd6b1242-2860-450d-abad-1ca603a16f40)

https://www.tinkercad.com/things/5M4UyYBgRPH-7432-quad-2-input-or-gate?sharecode=v5NsHIptAl-JgBzUaAZVW18XOLPlYQC5ay1_0E7kRKI


# Pin Description

| Pin No. | Symbol | Function                              |
| ------- | ------ | ------------------------------------- |
| 1       | 1A     | Input of 1st OR gate                  |
| 2       | 1B     | Input of 1st OR gate                  |
| 3       | 1Y     | Output of 1st OR gate (1A OR 1B)      |
| 4       | 2A     | Input of 2nd OR gate                  |
| 5       | 2B     | Input of 2nd OR gate                  |
| 6       | 2Y     | Output of 2nd OR gate (2A OR 2B)      |
| 7       | GND    | Ground (0V)                           |
| 8       | 3Y     | Output of 3rd OR gate (3A OR 3B)      |
| 9       | 3A     | Input of 3rd OR gate                  |
| 10      | 3B     | Input of 3rd OR gate                  |
| 11      | 4Y     | Output of 4th OR gate (4A OR 4B)      |
| 12      | 4A     | Input of 4th OR gate                  |
| 13      | 4B     | Input of 4th OR gate                  |
| 14      | Vcc    | Positive supply voltage (+5V typical) |

- Each gate gives a HIGH output when at least one input is HIGH.

- Power supply on Pin 14, Ground on Pin 7.

# 3. 7404- Hex inverter- NOT GATE

# Pin Diagram


![image](https://github.com/user-attachments/assets/8220418f-24f1-47ca-ba9d-9fe6467f8711)


![image](https://github.com/user-attachments/assets/ba0289c6-b410-46ce-bac8-91608014f86c)

https://www.tinkercad.com/things/1VF6mKArJow-7404-hex-inverter-not-gate

# Pin Description
| Pin No | Name | Function                              |
| ------ | ---- | ------------------------------------- |
| 1      | 1A   | Input of inverter 1                   |
| 2      | 1Y   | Output of inverter 1 (inverted 1A)    |
| 3      | 2A   | Input of inverter 2                   |
| 4      | 2Y   | Output of inverter 2 (inverted 2A)    |
| 5      | 3A   | Input of inverter 3                   |
| 6      | 3Y   | Output of inverter 3 (inverted 3A)    |
| 7      | GND  | Ground (0V)                           |
| 8      | 4Y   | Output of inverter 4 (inverted 4A)    |
| 9      | 4A   | Input of inverter 4                   |
| 10     | 5Y   | Output of inverter 5 (inverted 5A)    |
| 11     | 5A   | Input of inverter 5                   |
| 12     | 6Y   | Output of inverter 6 (inverted 6A)    |
| 13     | 6A   | Input of inverter 6                   |
| 14     | Vcc  | Positive supply voltage (+5V typical) |

- Each gate has 1 input and 1 output.

- Vcc and GND are on Pins 14 and 7 respectively.

# 4. 7400- Quad 2-input NAND gate 

# Pin Diagram

![image](https://github.com/user-attachments/assets/39ed22d7-d7d3-4919-97f2-26b5114a4625)


![image](https://github.com/user-attachments/assets/407d9f9a-dd87-4cd9-8271-6f8031ede7dd)


# Pin Description

| Pin | Symbol | Function                              |
| --- | ------ | ------------------------------------- |
| 1   | 1A     | Input A of Gate 1                     |
| 2   | 1B     | Input B of Gate 1                     |
| 3   | 1Y     | Output of Gate 1 (NAND of 1A & 1B)    |
| 4   | 2A     | Input A of Gate 2                     |
| 5   | 2B     | Input B of Gate 2                     |
| 6   | 2Y     | Output of Gate 2 (NAND of 2A & 2B)    |
| 7   | GND    | Ground (0V)                           |
| 8   | 3B     | Input B of Gate 3                     |
| 9   | 3A     | Input A of Gate 3                     |
| 10  | 3Y     | Output of Gate 3 (NAND of 3A & 3B)    |
| 11  | 4Y     | Output of Gate 4 (NAND of 4A & 4B)    |
| 12  | 4B     | Input B of Gate 4                     |
| 13  | 4A     | Input A of Gate 4                     |
| 14  | Vcc    | Positive Power Supply (+5V typically) |

- Each with 2 inputs (A & B) and 1 output (Y).

- Pin 14 is for power supply (Vcc = +5V), and Pin 7 is for Ground.

# 5.  7402- Quad 2-input NOR gate 

# Pin Diagram

![image](https://github.com/user-attachments/assets/bb832e91-2aeb-46e0-8849-da04a50bec79)


![image](https://github.com/user-attachments/assets/1644fd7a-bdbc-461b-9912-5b51ee6c45ad)


# Pin Description
| Pin No. | Pin Name | Description                  |
| ------- | -------- | ---------------------------- |
| 1       | 1A       | Input A of NOR Gate 1        |
| 2       | 1B       | Input B of NOR Gate 1        |
| 3       | 1Y       | Output of NOR Gate 1         |
| 4       | 2A       | Input A of NOR Gate 2        |
| 5       | 2B       | Input B of NOR Gate 2        |
| 6       | 2Y       | Output of NOR Gate 2         |
| 7       | GND      | Ground (0V)                  |
| 8       | 3Y       | Output of NOR Gate 3         |
| 9       | 3A       | Input A of NOR Gate 3        |
| 10      | 3B       | Input B of NOR Gate 3        |
| 11      | 4Y       | Output of NOR Gate 4         |
| 12      | 4A       | Input A of NOR Gate 4        |
| 13      | 4B       | Input B of NOR Gate 4        |
| 14      | Vcc      | Supply Voltage (+5V typical) |

- Each gate takes 2 inputs and gives 1 output based on NOR logic.

- Pin 14 supplies power; Pin 7 connects to ground.

# 6. 7486- Quad 2-input Exclusive-OR gate 

# Pin Diagram

![image](https://github.com/user-attachments/assets/e163eff0-ed64-4bba-b6af-d0f9e0b4f69b)


![image](https://github.com/user-attachments/assets/586c3c71-705a-4309-931c-1b7725cb2442)


# Pin Description
| Pin No. | Pin Name | Description                  |
| ------- | -------- | ---------------------------- |
| 1       | 1A       | Input A of Gate 1            |
| 2       | 1B       | Input B of Gate 1            |
| 3       | 1Y       | Output of Gate 1 (1A ⊕ 1B)   |
| 4       | 2A       | Input A of Gate 2            |
| 5       | 2B       | Input B of Gate 2            |
| 6       | 2Y       | Output of Gate 2 (2A ⊕ 2B)   |
| 7       | GND      | Ground (0V)                  |
| 8       | 3Y       | Output of Gate 3 (3A ⊕ 3B)   |
| 9       | 3A       | Input A of Gate 3            |
| 10      | 3B       | Input B of Gate 3            |
| 11      | 4Y       | Output of Gate 4 (4A ⊕ 4B)   |
| 12      | 4A       | Input A of Gate 4            |
| 13      | 4B       | Input B of Gate 4            |
| 14      | Vcc      | Supply Voltage (+5V typical) |

- Output is HIGH when only one input is HIGH.

- Commonly used in adders and parity checkers.

# 7.  74266 or 74LS266- Quad 2-input Exclusive-NOR gate 

# Pin Diagram

![image](https://github.com/user-attachments/assets/2e2d6ce2-6aae-462d-a091-aae2c1f68c12)


![image](https://github.com/user-attachments/assets/c852ab4c-e7cb-422d-8d69-364390a1e49a)


# Pin Description
| Pin No | Pin Name | Description                    |
| ------ | -------- | ------------------------------ |
| 1      | 1A       | Input A of EX-NOR Gate 1       |
| 2      | 1B       | Input B of EX-NOR Gate 1       |
| 3      | 1Y       | Output of EX-NOR Gate 1        |
| 4      | 2A       | Input A of EX-NOR Gate 2       |
| 5      | 2B       | Input B of EX-NOR Gate 2       |
| 6      | 2Y       | Output of EX-NOR Gate 2        |
| 7      | GND      | Ground (0V)                    |
| 8      | 3Y       | Output of EX-NOR Gate 3        |
| 9      | 3B       | Input B of EX-NOR Gate 3       |
| 10     | 3A       | Input A of EX-NOR Gate 3       |
| 11     | 4Y       | Output of EX-NOR Gate 4        |
| 12     | 4B       | Input B of EX-NOR Gate 4       |
| 13     | 4A       | Input A of EX-NOR Gate 4       |
| 14     | Vcc      | Supply Voltage (+5V typically) |

- Gates with open-collector outputs (requires pull-up resistor).

- Output is HIGH when inputs are the same.

# Applications of logic gates

| **Logic Gate** | **IC Number **           | **Applications**                                                                                                                           |
| -------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| **AND Gate**   | 7408                     | - Password verification circuits<br>- Industrial safety systems<br>- Enable control in microcontrollers<br>- Traffic light controllers     |
| **OR Gate**    | 7432                     | - Emergency alarm systems<br>- Elevator control systems<br>- Data routing in networks<br>- Lighting systems with multiple control switches |
| **NOT Gate**   | 7404                     | - Signal inversion in processors<br>- Logic level shifting<br>- Control logic for automatic systems<br>- Oscillator circuits               |
| **NAND Gate**  | 7400                     | - Used to build flip-flops<br>- Logic function implementation (universal gate)<br>- Alarm circuits<br>- Pulse generation                   |
| **NOR Gate**   | 7402                     | - Used in control logic circuits<br>- Universal gate for building any logic circuit<br>- Digital locks<br>- Frequency detectors            |
| **XOR Gate**   | 7486                     | - Parity checker and generator<br>- Half adders and full adders<br>- Error detection in communication<br>- Digital comparators             |
| **XNOR Gate**  | 74266                    | - Equality comparators<br>- Error checking circuits<br>- Phase detectors<br>- Digital data matching systems                                |














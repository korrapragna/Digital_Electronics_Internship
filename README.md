 # DIGITAL ELECTRONICS

# Table of Contents

- [What is Digital Electronics](#What-is-Digital-Electronics)

- [Applications of Digital Electronics](#Applications-of-Digital-Electronics).

- [Digital vs Analog Signals](#Digital-vs-Analog-Signals)

- [Number System](#Number-System)

- [Conversion between Number System](#Conversion-between-Number-System)

- [Basic Logic gates](#Basic-Logic-gates)

- [Integrated Circuits](#Integrated-Circuits)

- [Implementation of Logic gates](#Implementation-of-Logic-gates)

- [Implementation of Half Adder](#Implementation-of-Half-Adder)
  
- [Implementation of Full Adder](#Implementation-of-Full-Adder)

- [Implementation of Multiplexers](#Implementation-of-Multiplexers)
  
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
| INPUT A |INPUT B | OUTPUT Y    |
| -       | -      | ----------- |
| 0       | 0      | 0           |
| 0       | 1      | 0           |
| 1       | 0      | 0           |
| 1       | 1      | 1           |
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
|INPUT A |INPUT B | OUTPUT Y |
| -      | -      | ---------- |
| 0      | 0      | 0          |
| 0      | 1      | 1          |
| 1      | 0      | 1          |
| 1      | 1      | 1          |
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
| INPUT A | OUTPUT Y  |
| -       | --------- |
| 0       | 1         |
| 1       | 0         |
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
|INPUT A |INPUT B |(A.B)        | OUTPUT Y                  |
| -      | -      | ----------- | ------------------------- |
| 0      | 0      | 0           | 1                         |
| 0      | 1      | 0           | 1                         |
| 1      | 0      | 0           | 1                         |
| 1      | 1      | 1           | 0                         |
# 5.NOR GATE
# Symbol :
![image](https://github.com/user-attachments/assets/627f332b-e977-42de-9886-a492488e4d49)

# Function :

A NOR (Not OR) gate gives an output of 1 only when both inputs are 0.

It is the inverse of the OR gate.
# Truth Table :
|INPUT A | INPUT B | OUTPUT Y |
| -      | -       | ------- |
| 0      | 0       | 1       |
| 0      | 1       | 0       |
| 1      | 0       | 0       |
| 1      | 1       | 0       |
# 6.XOR GATE
# Symbol :

![image](https://github.com/user-attachments/assets/d9f9f1df-f2ad-4fe1-91de-bd90ceb47b5f)

# Function :
The XOR (Exclusive OR) gate gives an output of 1 only when the inputs are different.

Boolean Expression : Y = A ⊕ B = A̅·B + A·B̅

# Truth table :
|INPUT A |INPUT B | OUTPUT Y |
| -      | -      | ------- |
| 0      | 0      | 0       |
| 0      | 1      | 1       |
| 1      | 0      | 1       |
| 1      | 1      | 0       |

# 7.XNOR GATE :
# Symbol :

![image](https://github.com/user-attachments/assets/7f54ebf7-8a5a-48de-897e-bc60afc44ba0)

# Function :
The XNOR (Exclusive NOR) gate gives an output of 1 only when the inputs are the same.

Boolean Expression : Y = (A ⊕ B)̅ = A·B + A̅·B̅

# Truth table :
| INPUT A |INPUT B | OUTPUT Y |
| -       | -      | -------- |
| 0       | 0      | 1        |
| 0       | 1      | 0        |
| 1       | 0      | 0        |
| 1       | 1      | 1        |

# Integrated Circuits
# What is an Ic?
An IC (Integrated Circuit) is a small electronic device made of a semiconductor material (usually silicon) that contains a large number of tiny components like:

- Transistors

- Resistors

- Capacitors

- Diodes

# Types of logic gates and their IC numbers

| Logic Gate | IC Number (TTL Series) | Description                     | No. of Gates in IC | Pin Count |
| ---------- | ---------------------- | ------------------------------- | ------------------ | --------- |
| AND        | 7408                   | Quad 2-input AND gate           | 4                  | 14        |
| OR         | 7432                   | Quad 2-input OR gate            | 4                  | 14        |
| NOT        | 7404                   | Hex inverter (NOT gate)         | 6                  | 14        |
| NAND       | 7400                   | Quad 2-input NAND gate          | 4                  | 14        |
| NOR        | 7402                   | Quad 2-input NOR gate           | 4                  | 14        |
| XOR        | 7486                   | Quad 2-input Exclusive-OR gate  | 4                  | 14        |
| XNOR       | 74266 or 74LS266       | Quad 2-input Exclusive-NOR gate | 4                  | 14        |

# Applications of IC's
| Logic Gate Type | IC Number | Applications                                              | Number of Gates | Pin Count |
| --------------- | --------- | --------------------------------------------------------- | --------------- | --------- |
| AND Gate        | 7408      | Digital logic circuits, alarm systems, control systems    | 4               | 14        |
| OR Gate         | 7432      | Signal processing, data selection, switching circuits     | 4               | 14        |
| NOT Gate        | 7404      | Inverters, signal restoration, logic level conversion     | 6               | 14        |
| NAND Gate       | 7400      | Basic logic building blocks, flip-flops, control circuits | 4               | 14        |
| NOR Gate        | 7402      | Oscillators, pulse generators, digital logic designs      | 4               | 14        |
| XOR Gate        | 7486      | Parity checkers, adders, digital comparators              | 4               | 14        |
| XNOR Gate       | 74266     | Equality comparators, arithmetic circuits                 | 4               | 14        |

# 1. 7408-Quad 2-input AND gate

# Pin Diagram:

![image](https://github.com/user-attachments/assets/3bad826b-93f9-433e-9c82-41d3a635951b)

![image](https://github.com/user-attachments/assets/75d51c86-38e3-43ba-a62d-6abf5674be80)

![image](https://github.com/user-attachments/assets/2f6d6482-50e0-4d99-aadf-f5848119888a)

# Tinkercad Circuit: AND Gate using IC 7408

Link : [Open in Tinkercad](https://www.tinkercad.com/things/eDdC36KJHwt-7408-quad-2-input-and-gate)

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

Description

- Each AND gate outputs HIGH only if both inputs are HIGH.

- Power: Pin 14 (Vcc), Ground: Pin 7.

# 2. 7432-Quad 2-input OR gate

# Pin Diagram:

![image](https://github.com/user-attachments/assets/6be5005e-3926-4ac2-bca4-bec098b80c86)

![image](https://github.com/user-attachments/assets/dd6b1242-2860-450d-abad-1ca603a16f40)

![image](https://github.com/user-attachments/assets/874593f4-a76c-4b05-be1b-56a84728450a)

# Tinkercad Circuit: OR Gate using IC 7432

Link : [Open in Tinkercad](https://www.tinkercad.com/things/5M4UyYBgRPH-7432-quad-2-input-or-gate)

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

Description

- Each gate gives a HIGH output when at least one input is HIGH.

- Power supply on Pin 14, Ground on Pin 7.

# 3. 7404- Hex inverter- NOT GATE

# Pin Diagram

![image](https://github.com/user-attachments/assets/8220418f-24f1-47ca-ba9d-9fe6467f8711)

![image](https://github.com/user-attachments/assets/ba0289c6-b410-46ce-bac8-91608014f86c)

![image](https://github.com/user-attachments/assets/d545879f-7557-4a30-b6bd-8e34884fb7fb)

# Tinkercad Circuit : NOT Gate using IC 7404

Link : [Open 7404 Hex Inverter NOT Gate on Tinkercad](https://www.tinkercad.com/things/1VF6mKArJow-7404-hex-inverter-not-gate)

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

Description

- Each gate has 1 input and 1 output.

- Vcc and GND are on Pins 14 and 7 respectively.

# 4. 7400- Quad 2-input NAND gate 

# Pin Diagram

![image](https://github.com/user-attachments/assets/39ed22d7-d7d3-4919-97f2-26b5114a4625)

![image](https://github.com/user-attachments/assets/407d9f9a-dd87-4cd9-8271-6f8031ede7dd)

![image](https://github.com/user-attachments/assets/e72cba9a-1d8e-4820-9a42-f1c1a00a2241)

# Tinkercad Circuit : NAND Gate using IC 7400

[Open in Tinkercad](https://www.tinkercad.com/things/8wMx3LFda8G-7400-quad-2-input-nand-gate)

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

Description

- Each with 2 inputs (A & B) and 1 output (Y).

- Pin 14 is for power supply (Vcc = +5V), and Pin 7 is for Ground.

# 5.  7402- Quad 2-input NOR gate 

# Pin Diagram

![image](https://github.com/user-attachments/assets/882c548a-420d-40fc-a8cc-1eb4cbfaca61)

![image](https://github.com/user-attachments/assets/1644fd7a-bdbc-461b-9912-5b51ee6c45ad)

![image](https://github.com/user-attachments/assets/edbb2011-5c4e-42a8-9ad1-5bb7231f13fe)

# Tinkercad Circuit : NOR Gate using IC 7402

Link : [7402 Quad 2-Input NOR Gate on Tinkercad](https://www.tinkercad.com/things/ezbi74UdIu4-7402-quad-2-input-nor-gate)

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

Description

- Each gate takes 2 inputs and gives 1 output based on NOR logic.

- Pin 14 supplies power; Pin 7 connects to ground.

# 6. 7486- Quad 2-input Exclusive-OR gate 

# Pin Diagram

![image](https://github.com/user-attachments/assets/9c02be29-4ddc-4677-a6c0-a0f71201fcc1)

![image](https://github.com/user-attachments/assets/586c3c71-705a-4309-931c-1b7725cb2442)

![image](https://github.com/user-attachments/assets/a88f8cf6-bc7f-4f55-9d05-33b68757a3be)

# Tinkercad Circuit : XOR Gate using IC 7486

Link : [Open in Tinkercad](https://www.tinkercad.com/things/5Ir7WDrAO2X-7486-quad-2-input-exclusive-or-gate)

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

Description

- Output is HIGH when only one input is HIGH.

- Commonly used in adders and parity checkers.

# 7.  74266 or 74LS266- Quad 2-input Exclusive-NOR gate 

# Pin Diagram

![image](https://github.com/user-attachments/assets/458d0c5b-76bf-431a-8d5c-7fc25de5f0fa)

![image](https://github.com/user-attachments/assets/c852ab4c-e7cb-422d-8d69-364390a1e49a)

![image](https://github.com/user-attachments/assets/a8ede943-8cb3-4d21-8ba8-db44c7ba1720)

#  Tinkercad Circuit : XNOR Gate using IC 74LS66

Link : [Open in Tinkercad](https://www.tinkercad.com/things/hXoqtZrVHhK-74266-quad-2-input-exclusive-nor-gate-)

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

Description

- Gates with open-collector outputs (requires pull-up resistor).

- Output is HIGH when inputs are the same.

# Implementation of Logic gates

# AND gate using NAND gate 7400
![image](https://github.com/user-attachments/assets/744674bf-febb-46c0-a953-41be857c5e96)

# Tinkercad Link : 
[AND gate using NAND gate 7400 on Tinkercad](https://www.tinkercad.com/things/a1t5VJz6Hb3-and-gate-using-nand-gate-7400)

# OR gate using NAND gate 7400
![image](https://github.com/user-attachments/assets/ad943213-d1bb-4bb8-a97f-1b010100b284)

# Tinkercad Link : 
[OR Gate using NAND Gate - Tinkercad](https://www.tinkercad.com/things/4MVhqPxYb8F-or-gate-using-nand-gate-7400)

# NOT gate using NAND gate 7400
![image](https://github.com/user-attachments/assets/ec6dacee-4cf4-4f93-a56c-d7f277d17ea3)

# Tinkercad Link : 
[NOT Gate using NAND Gate (Tinkercad)](https://www.tinkercad.com/things/aatCVZAgsNE-not-gate-using-nand-gate-7400)

# AND gate using NOR gate 7402
![image](https://github.com/user-attachments/assets/91fce872-6f20-49d9-86f6-0e708b4b5963)

# Tinkercad Link : 
[AND Gate using NOR Gate (7402) - Tinkercad](https://www.tinkercad.com/things/jjga50hvkjJ-and-gate-using-nor-gate-7402)

# OR gate using NOR gate 7402
![image](https://github.com/user-attachments/assets/273c32b1-ac57-4d7a-85f0-9b6e8ce4d35b)

# Tinkercad Link : 
[Open OR Gate using NOR Gate (7402) in Tinkercad](https://www.tinkercad.com/things/iXXioJ5NSDX-or-gate-using-nor-gate-7402)

# NOT gate using NOR gate 7402
![image](https://github.com/user-attachments/assets/b519ef9d-e01e-400a-ba7a-58d6a9a1946a)

# Tinkercad Link : 
[NOT Gate using NOR Gate - Tinkercad](https://www.tinkercad.com/things/7SqApTzLLIG-not-gate-using-nor-gate-7402)

# Implementation of Half Adder

# Block Diagram
![image](https://github.com/user-attachments/assets/d12d4ab5-dd4d-4c0a-81da-53507936d953)
# Tinkercad Image
![image](https://github.com/user-attachments/assets/5228f63c-9c46-483c-a41a-710fda06c84f)

Link : [View Half Adder using NAND Gates on Tinkercad](https://www.tinkercad.com/things/3culvWwis9B-half-adder-using-nand-gates-7400)

# Half Adder using 7400 NAND IC Pins

| **Pin No.** | **Pin Name**        | **Connection / Function**              |
| ----------- | ------------------- | -------------------------------------- |
| 1           | 1A (Gate 1 Input A) | Input A                                |
| 2           | 1B (Gate 1 Input B) | Input B                                |
| 3           | 1Y (Gate 1 Output)  | Output of A NAND B (used for Carry)    |
| 4           | 2A (Gate 2 Input A) | Input A                                |
| 5           | 2B (Gate 2 Input B) | Input B                                |
| 6           | 2Y (Gate 2 Output)  | Output of A NAND B (used in Sum logic) |
| 7           | GND                 | Connect to Ground (0V)                 |
| 8–12        | Unused              | Not used in 2-gate configuration       |
| 13          | Not used            | –                                      |
| 14          | Vcc                 | Connect to +5V                         |

Description 

- Pin 3 provides the Carry output.

- Pin 6 can be used as part of Sum (XOR) if extended with additional NANDs.

# Truth Table 
| A | B | Sum | Carry |
| - | - | --- | ----- |
| 0 | 0 | 0   | 0     |
| 0 | 1 | 1   | 0     |
| 1 | 0 | 1   | 0     |
| 1 | 1 | 0   | 1     |

Logic Explanation:

- Sum is the result of A XOR B

- Carry is the result of A AND B

# Implementation of Full Adder

# Block Diagram
![image](https://github.com/user-attachments/assets/f8a5a8ef-6b52-4d4f-8e9b-3797bd0ef562)
# Tinkercad Image
![image](https://github.com/user-attachments/assets/2512f7f6-7372-4a5e-ab7f-7c34838c342e)

Link : 🔗 [Open Tinkercad Simulation](https://www.tinkercad.com/things/7cQNngEElA9-full-adder-using-nor-gate-7402)

# Full Adder using 7402 NAND IC Pins
| Pin No. | Function            | Gate No. | Description            |
| ------- | ------------------- | -------- | ---------------------- |
| 1       | A Input             | Gate 1   | First input of Gate 1  |
| 2       | B Input             | Gate 1   | Second input of Gate 1 |
| 3       | Output              | Gate 1   | Output of Gate 1       |
| 4       | A Input             | Gate 2   | First input of Gate 2  |
| 5       | B Input             | Gate 2   | Second input of Gate 2 |
| 6       | Output              | Gate 2   | Output of Gate 2       |
| 7       | **GND**             | –        | Ground (0V)            |
| 8       | Output              | Gate 3   | Output of Gate 3       |
| 9       | B Input             | Gate 3   | Second input of Gate 3 |
| 10      | A Input             | Gate 3   | First input of Gate 3  |
| 11      | Output              | Gate 4   | Output of Gate 4       |
| 12      | B Input             | Gate 4   | Second input of Gate 4 |
| 13      | A Input             | Gate 4   | First input of Gate 4  |
| 14      | **Vcc** (Power +5V) | –        | Positive power supply  |

Description 

- The IC contains 4 independent NOR gates.

- Power is supplied through Pin 14 (Vcc) and Pin 7 (GND).

- You can use these gates to build a full adder logic by combining multiple NOR operations.
# Truth Table 
| A | B | Cin | Sum | Cout |
| - | - | --- | --- | ---- |
| 0 | 0 | 0   | 0   | 0    |
| 0 | 0 | 1   | 1   | 0    |
| 0 | 1 | 0   | 1   | 0    |
| 0 | 1 | 1   | 0   | 1    |
| 1 | 0 | 0   | 1   | 0    |
| 1 | 0 | 1   | 0   | 1    |
| 1 | 1 | 0   | 0   | 1    |
| 1 | 1 | 1   | 1   | 1    |

# Implementation of Multiplexers
# What is a Multiplexer?
 A multiplexer (often abbreviated as MUX) is a digital electronic device that selects one input from multiple input signals and forwards it to a single output line. It acts like a digital switch.

@ Key Points:
- A multiplexer has multiple data inputs, one output, and select lines (also called control lines).

- The number of select lines determines how many inputs the multiplexer can handle.

- For example, a 2ⁿ-to-1 multiplexer has:

- 2ⁿ inputs

- 1 output

- n select lines
# Types of Multiplexers
| **Multiplexer Type** | **Number of Inputs** | **Number of Selection Lines** | **Number of Outputs** |
| -------------------- | -------------------- | ----------------------------- | --------------------- |
| 2:1 MUX              | 2                    | 1                             | 1                     |
| 4:1 MUX              | 4                    | 2                             | 1                     |
| 8:1 MUX              | 8                    | 3                             | 1                     |
| 16:1 MUX             | 16                   | 4                             | 1                     |
| 32:1 MUX             | 32                   | 5                             | 1                     |
| 64:1 MUX             | 64                   | 6                             | 1                     |

# 1. 2x1 Multiplexer
A 2:1 multiplexer (2-to-1 MUX) has 2 data inputs, 1 select line, and 1 output. Despite its simplicity, it has many practical applications in digital systems.
# Block Diagram
![image](https://github.com/user-attachments/assets/47de5c7e-97a9-485a-92c1-0266e0cbb791)

# Tinkercad Image
![image](https://github.com/user-attachments/assets/9de413d1-5d04-47e3-a1e8-7df1b2b62c23)

Link : [2:1 Multiplexer](https://www.tinkercad.com/things/bEsXioE9o1n-21-multiplexer)

# IC pin configuration
| **Pin No.** | **7404 (Hex Inverter)** | **7408 (Quad AND Gate)** | **7432 (Quad OR Gate)** |
| ----------- | ----------------------- | ------------------------ | ----------------------- |
| 1           | A1 (Input)              | A1 (Input)               | A1 (Input)              |
| 2           | Y1 (Output)             | B1 (Input)               | B1 (Input)              |
| 3           | A2 (Input)              | Y1 (Output)              | Y1 (Output)             |
| 4           | Y2 (Output)             | A2 (Input)               | A2 (Input)              |
| 5           | A3 (Input)              | B2 (Input)               | B2 (Input)              |
| 6           | Y3 (Output)             | Y2 (Output)              | Y2 (Output)             |
| 7           | **GND**                 | **GND**                  | **GND**                 |
| 8           | Y4 (Output)             | Y3 (Output)              | Y3 (Output)             |
| 9           | A4 (Input)              | B3 (Input)               | B3 (Input)              |
| 10          | Y5 (Output)             | A3 (Input)               | A3 (Input)              |
| 11          | A5 (Input)              | Y4 (Output)              | Y4 (Output)             |
| 12          | Y6 (Output)             | B4 (Input)               | B4 (Input)              |
| 13          | A6 (Input)              | A4 (Input)               | A4 (Input)              |
| 14          | **Vcc** (5V)            | **Vcc** (5V)             | **Vcc** (5V)            |

# Truth Table
| Select (S) | Input A | Input B | Output Y |
| ---------- | ------- | ------- | -------- |
| 0          | 0       | 0       | 0        |
| 0          | 0       | 1       | 0        |
| 0          | 1       | 0       | 1        |
| 0          | 1       | 1       | 1        |
| 1          | 0       | 0       | 0        |
| 1          | 0       | 1       | 1        |
| 1          | 1       | 0       | 0        |
| 1          | 1       | 1       | 1        |
# Applications 
- Data Selector
 
- Implementing Logic Gates

- Function Generator

- CPU Data Path Selection

# 2. 4x1 Multiplexer
A 4:1 multiplexer is a digital device that selects one of four input signals and passes it to a single output line, based on the values of two select lines.

# Block Diagram
![image](https://github.com/user-attachments/assets/df563e73-a0dd-452c-a0bf-b71da9a6a5af)

# Tinkercad Image
![image](https://github.com/user-attachments/assets/80ac0eab-7b8f-4e76-a777-d37ece8c5c4c)

Link : 🔗 [View on Tinkercad](https://www.tinkercad.com/things/7fDgLuKNeWr-4x1-multiplexer)

# IC pin configuration
| **Pin No.** | **7411 (3-input AND)** | **7404 (NOT)**          | **7432 (2-input OR)**  |
| ----------- | ---------------------- | ----------------------- | ---------------------- |
| 1           | 1A (Input, Gate 1)     | 1A (Input, Inverter 1)  | 1A (Input, OR Gate 1)  |
| 2           | 1B (Input, Gate 1)     | 1Y (Output, Inverter 1) | 1B (Input, OR Gate 1)  |
| 3           | 1C (Input, Gate 1)     | 2A (Input, Inverter 2)  | 1Y (Output, OR Gate 1) |
| 4           | 1Y (Output, Gate 1)    | 2Y (Output, Inverter 2) | 2A (Input, OR Gate 2)  |
| 5           | 2A (Input, Gate 2)     | 3A (Input, Inverter 3)  | 2B (Input, OR Gate 2)  |
| 6           | 2B (Input, Gate 2)     | 3Y (Output, Inverter 3) | 2Y (Output, OR Gate 2) |
| 7           | **GND**                | **GND**                 | **GND**                |
| 8           | 2C (Input, Gate 2)     | 4Y (Output, Inverter 4) | 3Y (Output, OR Gate 3) |
| 9           | 2Y (Output, Gate 2)    | 4A (Input, Inverter 4)  | 3A (Input, OR Gate 3)  |
| 10          | 3A (Input, Gate 3)     | 5Y (Output, Inverter 5) | 3B (Input, OR Gate 3)  |
| 11          | 3B (Input, Gate 3)     | 5A (Input, Inverter 5)  | 4Y (Output, OR Gate 4) |
| 12          | 3C (Input, Gate 3)     | 6Y (Output, Inverter 6) | 4A (Input, OR Gate 4)  |
| 13          | 3Y (Output, Gate 3)    | 6A (Input, Inverter 6)  | 4B (Input, OR Gate 4)  |
| 14          | **Vcc** (+5V)          | **Vcc** (+5V)           | **Vcc** (+5V)          |

# Truth Table
| S1 | S0 | Y (Output) |
| -- | -- | ---------- |
| 0  | 0  | D0         |
| 0  | 1  | D1         |
| 1  | 0  | D2         |
| 1  | 1  | D3         |

# Applications 
- Data Routing
  
- ALU Design
  
- Function Generation	
	
- Memory Addressing
  
- CPU Instruction Decoding

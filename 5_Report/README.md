# Abstract

Automobiles are growing in huge numbers in todays modern world. Inorder to constitute the overall features of the vehicle system, many advanced features contribute. Wiper system is an integral part of traditional as well as advanced vehicular systems which is a must in all the cars, buses, trucks etc.Windscreen wipers, windshield wipers or wiper blades  are devices used to remove rain, snow, ice, washer fluid, water, and/or debris from a vehicle's front window.The majority of motor vehicles, including cars, trucks, buses, locomotives, watercraft with enclosed cabins, and some aircraft, are fitted with one or more such wipers, which are usually legal requirements.The wiper consists of a metal arm with a pivoting end and a long rubber blade attached to the other end. In most of the vehicles, windscreen washer is implemented to enhance the overall functioning of the wiper system and improve visibility of driving and can be considered as an integral part of the vehicle safety system.
## Introduction

Wiper system is automatically ON during the time of rainfall. The senor is fixed in the vehicle glass. The conductive (Touch) sensor is used in this project. It senses the rainfall and giving control signal to the control unit. The control unit activates the wiper motor automatically.

## Components Used

## Stm32

The STM32 family of 32-bit microcontrollers based on the Arm® Cortex®-M processor is designed to offer new degrees of freedom to MCU users. It offers products combining very high performance, real-time capabilities, digital signal processing, low-power / low-voltage operation, and connectivity, while maintaining full integration and ease of development.

![image](https://user-images.githubusercontent.com/102678112/167770911-b81487e4-ff98-461d-ad48-6cf34fb3f297.png)

## Servo Motor

A servomotor is a rotary actuator or linear actuator that allows for precise control of angular or linear position, velocity and acceleration. It consists of a suitable motor coupled to a sensor for position feedback.

![image](https://user-images.githubusercontent.com/102678112/167772572-4d88ecf4-1bdf-468e-a997-ee7a3d892c26.png)


## Resistors

A resistor is a passive two-terminal electrical component that implements electrical resistance as a circuit element. In electronic circuits, resistors are used to reduce current flow.

![image](https://user-images.githubusercontent.com/102678112/167771801-68dfad5d-0ba3-4eec-a920-124934a40410.png)


## Capacitor

A capacitor is a device that stores electrical energy in an electric field. It is a passive electronic component with two terminals. The effect of a capacitor is known as capacitance.

![image](https://user-images.githubusercontent.com/102678112/167771908-31d64fea-4c18-4444-97e0-68cf25ac7c54.png)

## LED's

A light-emitting diode is a semiconductor light source that emits light when current flows through it. Electrons in the semiconductor recombine with electron holes, releasing energy in the form of photons.

![image](https://user-images.githubusercontent.com/102678112/167772029-5ac11090-643f-4a59-aff2-b1d448853f75.png)

## Cables and Connector

A cable, also known as a cord, plug, or connector transmits power or data between devices or positions, which is covered in plastic by one or more wires.

![image](https://user-images.githubusercontent.com/102678112/167772180-8ae89217-0607-4c44-b4ff-9f2be223eb10.png)

## Push Button

A push-button or simply button is a simple switch mechanism to control some aspect of a machine or a process. Buttons are typically made out of hard material, usually plastic or metal. 

![image](https://user-images.githubusercontent.com/102678112/167772326-b28c886c-9916-49bc-9325-9d8650434ced.png)

## High Level Requirements

| ID | Description | Status |
|----|--------------|-------|
| HLR01 | Detecting rainfall and active automobile rain wiper | Implemented |
| HLR02 | It operate manually | Implemented |
| HLR03 | Displaying the information in led | Implemented |

## Low Level Requirements

| ID | Description | Status |
|----|--------------|--------|
| LLR01 | It work functionally according to outside water | Implemented |
| LLR02 | Consume less power | Implemented |

## 4W's and 1H

## What:
Wipers system are operated by an electric motor. The electric motor is attached to a worm gear, which transmits the necessary force to a long rod that sets the wiper arms in motion.

##Why
The main purpose of the wiper system is to clean the windscreen sufficiently to provide suitable visibility at all times.

## When 
American inventor Mary Anderson received credit for the first operational windshield wiper, back in 1903. Anderson's “window cleaning device” used a rubber squeegee blade on an arm, operated via a hand-cranked lever from inside the vehicle.

## Where
Wipers system can be activated by a lever located to the right of the steering wheel. Pulling the lever down should activate the windshield wipers on their lowest setting

## How
When we turn the wiper on, the wiper switch sends the signal to the control module. The control module operates the wiper relay. The relay sends 12-volt power to the wiper motor.

## Structural Diagram
![image](https://user-images.githubusercontent.com/102678112/167782772-24d774f1-a923-49f2-9fd7-17ac3e11f276.png)

## Circuit Diagram 

## Block Diagram
![Screenshot 2022-05-11 151850](https://user-images.githubusercontent.com/102678112/167821983-2b7912ca-377e-465f-b4d3-66c1d0bdda04.png)


## Flow Chart
![Screenshot 2022-05-11 151527](https://user-images.githubusercontent.com/102678112/167821169-4e4573ab-eaad-4d7b-a583-3ea9ade98fe0.png)

# TEST CASES and Corresponding Output

## High Level Test Cases
| Test ID | Description | Exp.i/p | Exp.o/p | Actual o/p | STATUS |
| --------|:------------|:--------|:--------|:-----------|:-------------|
| 1 | check if the BUTTTON is pressed  | program execution | Microcontroller/Engine starts | LED ON(RED)| PASS |
| 2 | check if the BUTTTON is pressed  | program execution | WIPER starts | LED ON(BLUE)| PASS |
| 3 | check if the BUTTTON is pressed  | program execution | WIPER starts | LED ON(GREEN)| PASS |
| 4 | check if the BUTTTON is pressed  | program execution | WIPER starts | LED ON(ORANGE)| PASS |
| 5 | check if the BUTTTON is pressed  | - | Microcontroller/Engine stops | LED TURNED OFF| PASS |


## Low Level Test Cases
| Test ID | Description | Exp.i/p | Exp.o/p | Actual o/p | STATUS |
| --------|:------------|:--------|:--------|:-----------|:-------------|
| 1 | check if the BUTTTON is pressed  | program execution | Microcontroller/Engine starts | LED ON(RED)| PASS |
| 2 | check if the BUTTTON is pressed again | program execution | WIPER starts and speed of wiper is slow | LED ON(BLUE)| PASS |
| 3 | check if the BUTTTON is pressed again | program execution | WIPER starts and speed of wiper is moderate | LED ON(GREEN)| PASS |
| 4 | check if the BUTTTON is pressed again | program execution | WIPER starts and speed of wiper is good | LED ON(ORANGE)| PASS |
| 5 | check if the BUTTTON is pressed again | - | Microcontroller/Engine stops | LED TURNED OFF| PASS |

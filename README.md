# Smart Autonomous Paper Dispensing System with Digital Payment Integration

A compact vending machine that dispenses A4 paper sheets after a UPI payment. Final-year B.Tech Mechatronics capstone project (AY 2026-27), Rajarambapu Institute of Technology.

> Team project. **My role: payment integration** (dynamic UPI QR generation and payment confirmation).

## Problem
College stationery shops usually give around 100 sheets per student. The shopkeeper counts the sheets and collects payment by hand, which causes long queues, counting errors, and wasted time at peak hours.

## Solution
A machine that works like a small vending machine. The user enters the number of sheets, pays through a UPI QR code, and the machine counts and dispenses exactly that many A4 sheets. It will be placed on our department floor for students to use during busy assignment submission times.

## How it works
1. The user selects the number of sheets on the keypad.
2. A dynamic UPI QR code is generated for the exact amount.
3. The user pays with any UPI app and the payment is verified.
4. The stepper-motor pickup mechanism feeds the paper.
5. Sensors count the sheets and check for jams.
6. The sheets are dispensed.
7. The transaction is logged to an IoT dashboard.

## Hardware
- Microcontroller: ESP32
- Paper pickup: stepper motor mechanism ([stepper driver model])
- Sensors: [sensor type] for sheet counting and jam detection
- Input and display: keypad and display screen
- Connectivity: Wi-Fi (ESP32) for IoT monitoring

## Software
- Embedded control logic for user input, payment verification, sensors, motors, dispensing, and error handling
- Payment: dynamic UPI QR generation for the entered amount ([how payment is confirmed])
- IoT dashboard for transaction logging and inventory monitoring ([platform used])
- Price per sheet: [1 rupees]

## Design targets
These are the goals set for the project, not measured results.
- More than 500 transactions per day
- Less than 3 seconds from payment to dispense
- High sheet-counting accuracy
- Sensor-based anti-jam detectio

## Images
Add these inside an `images` folder.
- Circuit diagram: `images/circuit-diagram.png`
- Concept drawings: `images/concept-drawing.png`
- Outer body design: `images/outer-body.png`
- Photo of the machine: `images/machine.jpg`

![Circuit diagram](images/circuit-diagram.png)

## My contribution
- Dynamic UPI QR generation for the amount entered
- Payment confirmation and the signal to the motors

## Methodology
Problem identification, requirements, design, component selection, prototype, programming, testing, performance evaluation, optimization, and final prototype.

## Team
- Abhishek Shinde
- Atharv Vader
- Mandar Bhingardeve
- Omesh Pawar
- Shashank Nandwalkar

Project guide: Prof. Onkar Mestry

## Status
Final assembly and fittings in progress. The machine will be put into use in our department next week.

## Limitations
- Designed for A4 paper (70-100 GSM)
- Long-term reliability is not tested yet, as the machine goes into use next week

## Future improvements
- RFID payment
- Refund on a failed dispense
- Low-stock alerts on the IoT dashboard

# car-parking-fpga
FSM-based car parking gate system in Verilog, deployed on Nexys DDR4. MIT Manipal DSD Lab, 2025.

# Car Parking Management System on FPGA

FSM-based parking gate controller synthesised and deployed 
on a Nexys DDR4 FPGA board.

## Features
- Password-authenticated FSM controlling gate access
- IR entry/exit sensor interfacing with debouncing and edge detection
- PWM generation for servo gate actuation
- Live slot count on 7-segment display
- Full RTL synthesis and behavioural simulation in Vivado

## Modules
- debounce — cleans IR sensor input
- edge_detector — generates single-cycle pulse on sensor trigger
- password_fsm — validates 4-bit switch input against stored password
- car_counter — tracks available slots (max 9)
- servo_pwm — generates PWM signal for servo gate
- seven_seg_display — drives 7-segment with slot count

## Hardware
- Nexys DDR4 FPGA board
- IR sensors (entry and exit)
- Servo motor for gate
- 7-segment display

## Status
Completed — December 2025
Synthesised, simulated and deployed on physical FPGA hardware.
Verilog HDL was written with AI assistance; integration, 
pin constraints and hardware testing done by the team.

## Files
- DSD_report.pdf — full report with RTL schematic, 
  simulation waveforms and Verilog source code

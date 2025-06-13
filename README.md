# Vehicle-Control-Using-CAN-Protocol

Vehicle Control using CAN Protocol – LPC2129 Project

This project simulates a basic vehicle communication system using the **CAN (Controller Area Network) protocol** on an **LPC2129 microcontroller**.

## Key Features:
- Microcontroller: **LPC2129 (ARM7TDMI-S core)**
- Uses **CAN1 peripheral** for transmitting and receiving messages
- Controls vehicle subsystems like:
  - Engine start/stop
  - Headlights
  - Brake signal
- Interrupt-based CAN message handling
- Message filtering and error handling supported

## Hardware & Debug Tools Used

- Microcontroller : LPC2129 (ARM7TDMI-S)
- CAN Transceiver : MCP2551
- CAN Analysis Tool : Vector CANalyzer (with Vector hardware board)
- Debug Output : UART Serial Monitor for CAN message logs


## Project Files:
- main.c – Application logic for vehicle control
- can_init.c – CAN1 initialization for LPC2129
- startup.s – Startup file for ARM7
- README.md – Project overview 

## How It Works:
- CAN1 is configured with a 125kbps or 250kbps baud rate
- Nodes send and receive messages using standard IDs
- Message filtering ensures that only relevant subsystem commands are processed
- LEDs / UART used to indicate command actions.

# RFID Access Control System

A smart access control system prototype built into a physical diorama, featuring multiple RFID scanners and automated door lock control.

## Overview

This project implements an RFID-based access control system designed for demonstration and prototyping purposes. The system is integrated into a physical diorama, providing a visual and interactive representation of how RFID access control works in real-world applications.

## System Components

### Hardware
- RC522 RFID Scanners (x4) - RFID card readers positioned on the diorama
- 5V Relay Module - Controls the door lock mechanism
- Green LED - Access granted indicator (physical)
- Red LED - Access denied indicator (physical)
- Door Lock Mechanism - Electromagnetic or solenoid lock

### Software
- File-based storage system for authorized RFID card data (local storage file)
- Access control logic with authentication validation (software controller)

## How It Works

### Workflow

1. Tap: A user taps an RFID card on one of the 4 RC522 scanners located on the diorama.

2. Verify: The system reads the card's unique identifier and checks it against the authorized IDs stored in a local file (memory/storage file).

3. Respond: The script processes the authentication and returns a response:
   - `GRANTED` - Card is authorized
   - `DENIED` - Card is not authorized

4. Actuate: Based on the response:
   - If GRANTED:
     - Physical green LED activates to indicate successful authentication
     - 5V relay triggers to open the door lock
     - Door remains unlocked for 5 seconds before automatically relocking
   - If DENIED:
     - Physical red LED activates to indicate failed authentication
     - Failed attempt is logged for security monitoring

## Features

- Multi-Scanner Support: Four independent RFID scanners for flexible access point placement
- Visual Feedback: Physical LED indicators provide immediate visual confirmation of access status
- Automatic Relocking: Door automatically relocks after 5 seconds for enhanced security
- Access Logging: Failed access attempts are logged for security auditing
- File-Based Storage: Simple and portable data storage for authorized cards (local file)

## 3D Diorama

The project includes a physical 3D diorama model (`3d Diorama.blend`) created in Blender, which houses all the hardware components and provides a realistic demonstration environment.

## License

This project is open source. Please refer to the repository for license details.

## Contributing

Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to contribute to this project.
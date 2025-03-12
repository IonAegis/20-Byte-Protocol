# 20-Byte Protocol

## Overview
The **20-Byte Protocol** is an ultra-lightweight networking protocol designed for **efficient communication with minimal resource consumption**. Unlike traditional routing protocols, it uses a **tag-based forwarding mechanism**, allowing devices to act as **lightweight routers** without maintaining large routing tables. This enables **highly scalable, decentralized networks** with **low RAM and CPU usage**, making it ideal for **IoT, mesh networks, and secure communications**.

## Key Features
- **Layer 4 Protocol**: Primarily operates at Layer 4 but can function as its own Layer 3 service when necessary.
- **Tag-Based Forwarding**: Devices relay packets based on tag-matching instead of conventional IP-based routing.
- **Fixed 20-Byte Packet Structure**: Minimal processing overhead and optimized efficiency.
- **Scalability**: Works well in decentralized, self-forming networks.
- **Low Power Consumption**: Ideal for embedded and IoT devices.
- **Security Potential**: Enables anonymous routing and encrypted overlays.

## Packet Structure
| Field         | Size (Bytes) | Description                                     |
|--------------|------------|-------------------------------------------------|
| Header       | 2          | Identifies the protocol version and type       |
| Source ID    | 4          | Unique identifier for the sending device       |
| Destination  | 4          | Target device or broadcast group               |
| Tags         | 6          | Label-based routing mechanism for forwarding   |
| Payload Hash | 2          | Ensures data integrity and quick validation    |
| Payload      | 2          | Minimal in-packet payload for metadata use     |

## Installation & Usage
1. **Clone the repository:**
   ```sh
   git clone https://github.com/YOUR-USERNAME/20-Byte-Protocol.git
   cd 20-Byte-Protocol

## Compile and run the reference implementation:
  make
./protocol_simulation

## License
This project is released under the Mozilla Public Licene 2.0 with a No-Commercial-Use clause, ensuring open access while preventing unauthorized commercialization.

## Future Roadmap
* Optimization for ultra-low-bandwidth environments
* AI-driven network path optimization
* Integration with modern secure networking standards

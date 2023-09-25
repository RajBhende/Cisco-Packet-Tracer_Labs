# Network Topology in Cisco Packet Tracer

## Description

This repository contains a network topology designed in Cisco Packet Tracer that connects the ACCOUNTS and DELIVERY departments. The network setup includes the following components:

- Two PCs in the ACCOUNTS department.
- Two PCs in the DELIVERY department.
- Switches to connect the PCs within each department.
- Routers for interdepartmental communication.
- Proper IP addressing using the network address 192.168.40.0.

## Topology Diagram

![Network Topology Diagram](https://github.com/RajBhende/Cisco-Packet-Tracer_Labs/assets/91026796/7201bab7-4037-4bdf-8dc0-41faf4dcd34c)

## Configuration Details

### ACCOUNTS Department

- PCs:
  - PC1: IP Address - 192.168.40.2, Subnet Mask - 255.255.255.0, Gateway - 192.168.40.1
  - PC2: IP Address - 192.168.40.3, Subnet Mask - 255.255.255.0, Gateway - 192.168.40.1
- Switch: Connects PC1 and PC2.

### DELIVERY Department

- PCs:
  - PC3: IP Address - 192.168.40.131, Subnet Mask - 255.255.255.128, Gateway - 192.168.40.1
  - PC4: IP Address - 192.168.40.132, Subnet Mask - 255.255.255.128, Gateway - 192.168.40.1
- Switch: Connects PC3 and PC4.

### Interdepartmental Connectivity

- Routers:
  - Router1:
    - Interface GigabitEthernet0/0: IP Address - 192.168.40.0, Subnet Mask - 255.255.255.128 (ACCOUNTS Department)
    - Interface GigabitEthernet0/1: IP Address - 192.168.40.128, Subnet Mask - 255.255.255.128 (DELIVERY Department)

## Testing Connectivity

To test connectivity between the ACCOUNTS and DELIVERY departments, you can use the following commands on the PCs:

- From a PC in the DELIVERY department (e.g., PC2):

ping 192.168.40.2 # Ping PC1 in ACCOUNTS department
ping 192.168.40.3 # Ping PC2 in ACCOUNTS department

- From a PC in the ACCOUNTS department (e.g., PC1):

  ping 192.168.40.130 # Ping PC3 in DELIVERY department
  ping 192.168.40.131 # Ping PC4 in DELIVERY department


  
## Author

- Raj Bhende

## Accessing the Cisco Packet Tracer File

To open and explore this network topology, follow these steps:

1. **Download Cisco Packet Tracer**: If you haven't already, download and install Cisco Packet Tracer from the [official website](https://www.netacad.com/courses/packet-tracer).

2. **Open Cisco Packet Tracer**: Launch the Cisco Packet Tracer application on your computer.

3. **Open the Topology File**:
   - In Cisco Packet Tracer, go to the "File" menu.
   - Select "Open."
   - Locate and select the Packet Tracer file provided in this repository (e.g., `network_topology.pkt`).

4. **Explore the Topology**: Once the file is open, you can interact with and explore the network topology. You can view the configurations of devices, connections, and test connectivity between departments.

Please note that this file is for educational and demonstration purposes. Make sure you have the necessary software (Cisco Packet Tracer) installed on your computer to view and work with the topology.

If you encounter any issues or have questions, feel free to reach out for assistance.










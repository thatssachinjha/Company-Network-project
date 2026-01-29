# Company-Network-Implementation-CCNA

1. Project Overview
This project is a network-based enterprise solution designed using Cisco Packet Tracer.
It simulates a real-world company network where multiple branches located at different places are interconnected using WAN technology, while internal communication inside each branch is handled using LAN switching.

The main aim is to:
  Provide secure communication
  Ensure department-wise separation
  Enable efficient routing between different locations
  Reduce IP address wastage using subnetting

The project uses:
  Routing Information Protocol (RIP) for routing
  VLANs for LAN switching and security
  Password-protected routers for access control

2. Network Architecture
2.1 Company Structure (Assumed Scenario)
The company has five locations:
  Delhi (Head Office)
  Nirman Vihar
  Dwarka
  Vaishali
  Ghaziabad

Role of Delhi Router
  Acts as the main headquarters
  Connects all branch routers
  Contains multiple departments

Implements VLANs and trunking
  Most secured router in the network
  All routers are interconnected using serial WAN links, forming a Wide Area Network (WAN).

3. Devices Used
The following network devices are used:

Routers (Cisco 1841)
  Perform inter-network communication
  Implement RIP routing
  Maintain routing tables
  Password protected for security

Switches (Cisco 2960)
  Used for LAN connectivity
  Enable VLAN creation
  Provide efficient switching using MAC addresses

End Devices
  PCs
  Laptops
  Servers
  Wireless Router
  Used in Vaishali network
  Allows laptops to connect wirelessly

4. Routing Protocol – RIP
Why RIP?
  RIP (Routing Information Protocol) is chosen because:
  It is simple
  Easy to configure
  Suitable for small to medium networks

RIP Characteristics
  Distance Vector Protocol
  Metric: Hop Count
  Maximum hop count: 15
  Hop count 16 = unreachable
  Sends updates every 30 seconds
  Administrative Distance: 120

Function in the Project
  Automatically shares route information between routers
  Helps routers select the best path
  Ensures communication between all branches

5. LAN Switching & VLAN Implementation
  VLAN (Virtual LAN)
  VLANs are implemented mainly in the Delhi Head Office to separate departments.

Departments (VLANs Created)
  Technical Department
  HR Department
  Finance Department
  Other Staff

Advantages of VLANs
  Improves network security
  Prevents unauthorized access
  Reduces broadcast traffic
  Logical separation without extra hardware

Trunking
  Trunk ports are used to:
  Allow multiple VLANs to pass through one link
  Enable communication between Manager, CEO, and HR
  Inter-VLAN communication is handled using routing.

6. IP Addressing & Subnetting
  IP Addressing
  Different Class A, B, and C IP addresses are used
  Each network has a unique IP range
  No IP address is repeated

Subnetting
  Used to:
  Reduce IP wastage
  Improve network efficiency
  Separate networks logically
  Each branch and department has its own subnet.

7. Security Features
  The network is designed with multiple security measures:
  Router passwords (Console, VTY, Enable)
  VLAN separation
  Controlled access between departments
  Limited broadcast domains
  Logical topology implementation

This prevents:
  Unauthorized access
  Data leakage between departments
  Network misuse

8. Project Working (Communication Flow)
  Inside a Branch
  PCs communicate via switches
  Same VLAN → direct communication
  Different VLAN → routing required
  Between Branches

Data travels:
  PC → Switch → Router → WAN → Router → Switch → PC
  RIP determines the best route
  Verification

Connectivity tested using:
  Ping
  Simulation mode
  Successful communication between:
  Same network
  Different networks
  Different VLANs
  Wired & wireless devices

9. Effectiveness of the Project
This project provides:

✔ Secure WAN communication
✔ Easy troubleshooting
✔ Scalability (up to 15 hops with RIP)
✔ Department-wise isolation
✔ Real-time enterprise simulation
✔ Reduced data redundancy

10. Applications / Use Cases
  Small to Medium Enterprises (SMEs)
  Multi-branch organizations
  Educational labs (CCNA practice)
  Network design demonstrations

11. Conclusion
  This project successfully demonstrates:
  Routing using RIP
  LAN switching with VLANs
  Enterprise-level security concepts
  Realistic WAN-LAN integration

It reflects how a real organization can securely connect multiple offices while maintaining efficient, scalable, and manageable networking.

If you want, I can now:

🔹 Prepare a viva answer version

🔹 Create a 2–3 minute explanation

🔹 Explain Packet Tracer configuration commands

🔹 Rewrite this as a final report conclusion

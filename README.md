# Network-Simulation

This project aims to simulate a simple computer network using socket connections to emulate communication between end systems and routers. The focus is on building a basic network infrastructure to understand routing algorithms and packet forwarding.

## Introduction

The project is divided into two main components:

1. **Simple End System:** Represents individual devices in the network with basic functionalities such as initialization, sending messages, and receiving messages.

2. **Simple Router:** Nodes in the network capable of connecting multiple end systems and forwarding messages between them. Includes functionalities for managing forwarding tables and routing protocols.

## Simple End System

End systems have the following functions:

- **Initialize:** Activates the end system, establishes a socket connection to the next hop, and broadcasts its existence to the network.
- **Send:** Attempts to send a message to a destination IP address with a specified TTL (Time To Live) through the network.
- **Receive:** Displays received messages and relevant information on the system's output.

## Simple Router

Routers connect multiple end systems and facilitate message forwarding. Key functionalities include:

- **Forwarding Tables:** Initially empty, routers build forwarding tables based on received messages and learn the IP addresses of neighboring routers.
- **Multi-Network Routing:** Routers connect networks together, share routing information with neighboring routers, and update forwarding tables accordingly.

## Routing Algorithms

Two routing algorithms are implemented:

- **OSPF (Open Shortest Path First):** A monitor node periodically retrieves routing tables from all routers, uses Dijkstra's algorithm to minimize hops, and updates routing tables accordingly.
- **RIP (Routing Information Protocol):** Distance vector advertisements are sent between routers to update state tables and propagate updates through the network.

## Implementation Details

- **Programming Language:** Python
- **Dependencies:** None

## Conclusion

This project provides hands-on experience in network simulation, routing algorithms, and socket programming. By simulating basic network components and implementing routing protocols, participants gain insights into the functioning of computer networks.


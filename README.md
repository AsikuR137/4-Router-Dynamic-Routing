# 4-Router-Dynamic-Routing
4-router dynamic routing project using RIP with LANs and point-to-point links for end-to-end connectivity
# 4-Router Dynamic Routing Project

## Project Overview
This project demonstrates a **dynamic routing setup** with 4 interconnected routers. The goal is to allow seamless communication between all PCs connected to the routers without manually configuring routes on each router.  

Dynamic routing protocols automatically share routing information between routers, making the network scalable and easy to manage.

---

## Network Design
- **Routers:** 4 (Router1, Router2, Router3, Router4)  
- **LAN IP Address Block:** `192.168.1.0/24`  
- **Router-to-Router Links:** `10.0.1.0/30`  
- **Subnetting:**  
  - Each LAN has a subnet from `192.168.1.0/24`  
  - Each point-to-point router link uses a /30 subnet for efficient IP usage  
- **PCs:** Connected to each router to test end-to-end connectivity.

---

## Routing Protocol
- **Protocol Used:** RIP (Routing Information Protocol)  
- **Why Dynamic Routing:**  
  - Automatically updates routing tables when the network changes.  
  - Reduces manual configuration and errors.  
  - Suitable for larger or evolving networks where static routing is impractical.

---

## Configuration Steps
1. Assign IP addresses to all router interfaces and PCs:  
   - LAN interfaces: `192.168.1.x/24`  
   - Router-to-router interfaces: `10.0.1.x/30`  
2. Enable RIP on each router.  
3. Advertise connected networks using the routing protocol.  
4. Verify connectivity:  
   - Ping PCs on different routers.  
   - Check routing tables to ensure all routes are shared.

---

## Challenges & Solutions
- **Problem:** PCs connected to Router3 initially could not communicate with other networks.  
- **Solution:** Verified interface configurations, ensured all networks were advertised in RIP, and checked routing tables.

---

## Key Learnings
- Practical experience with dynamic routing protocols.  
- Understanding of subnetting, IP addressing, and multi-router topology.  
- Troubleshooting real-world network connectivity issues.  
- Insight into the advantages of dynamic routing over static routing.

---

## Conclusion
This project successfully demonstrates a functional **multi-router dynamic routing network**, showing the efficiency and reliability of dynamic routing in scalable networks.

---

## Author
**Asikur Rahman**  
BSc in Electronics and Communication Engineering  
Hajee Mohammad Danesh Science and Technology University, Dinajpur

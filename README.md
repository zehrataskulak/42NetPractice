*This project has been created as part of the 42 curriculum by ztaskula.*

# NetPractice

## Overview

NetPractice is a core module within the 42 school curriculum focused on demystifying the foundational concepts of computer networking. Through a custom web-based simulator, participants must troubleshoot and repair 10 broken network topologies. 

The project serves as a practical introduction to the TCP/IP stack. By progressing through increasingly complex levels, students develop hands-on experience in calculating subnets, configuring device interfaces, and establishing correct routing paths to ensure seamless communication between internal hosts and the external internet.

## Getting Started

### Launching the Simulator

The exercises are completed via a local web interface. To set up the environment, follow these steps in your terminal:

1. Download and extract the project archive:
   ```bash
   tar -xvf net_practice.1.9.tgz
   cd net_practice
   ```
2. Execute the startup script:
   ```bash
   ./run.sh
   ```
3. The training interface will automatically launch in your default web browser. 
   *(Note: If browser security policies block the script, you can manually start a server using `python3 -m http.server 49242` and navigate to `http://localhost:49242`).*

### Workflow & Validation

In each level, your objective is to fill in the unshaded boxes (IP addresses, subnet masks, and routing rules) until all network goals are met.
- Use the **[Check again]** button to test your current topology.
- Once all goals indicate "OK - Congratulations!!", save your progress by clicking the **[Get my config]** button.

### Submission Requirements

To be successfully evaluated during your defense, you must download the configuration file for all 10 levels. **All 10 exported files must be placed directly at the root of your Git repository.** The evaluation cannot proceed without these files.

## Resources & Knowledge Base

### Core Networking Concepts

Successfully completing this project requires a solid understanding of the following theoretical concepts:

- **IPv4 Architecture:** The structure of IP addresses and how data packets travel across interconnected networks.
- **Subnetting (CIDR Notation):** Dividing large networks into smaller sub-networks, calculating block sizes, and utilizing logical AND operations to find Network IDs.
- **Reserved Addresses:** Understanding why the first IP (Network Address) and the last IP (Broadcast Address) in a subnet block cannot be assigned to standard host interfaces.
- **Routing Mechanics:** Formulating routing tables (`Target Network => Next Hop`) and setting up default routes (`0.0.0.0/0`) for external traffic or internet gateways.
- **Hardware Layering (OSI Model):** The distinction between Layer 2 devices (Switches, which connect devices within the same subnet via MAC) and Layer 3 devices (Routers, which bridge different subnets via IP).

### Useful References

- [NetPractice Walkthrough by imyzf](https://medium.com/@imyzf/netpractice-2d2b39b6cf0a) — Practical hints and strategies for conquering each topology.
- [Networking Guidelines by toufa7](https://toufa7.medium.com/netpractice-guidelines-6341b8309f38) — A great breakdown of the theoretical knowledge required for the project.
- [Subnetting & IP Addressing Explained (Video)](https://www.youtube.com/watch?v=HQUw0CfQWAM) — Excellent visual representation of subnet logic and binary math.

### AI Usage Declaration

Artificial Intelligence tools were utilized during the learning and development phases of this project for:
- **Troubleshooting & Debugging:** Identifying overlapping subnet errors, resolving "No forward/reverse way" routing loops, and understanding asymmetric masking.
- **Mathematical Verification:** Confirming binary AND calculations for Network IDs and verifying usable IP block ranges.
- **Documentation:** Assisting in drafting, structuring, and refining this README file to ensure clarity and compliance with subject requirements.
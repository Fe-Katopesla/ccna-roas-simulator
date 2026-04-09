# CCNA Layer 3 Router-on-a-Stick Simulator

[![Live Demo](https://img.shields.io/badge/Live-Demo-00ff41?style=for-the-badge&logo=github&logoColor=black)](https://fe-katopesla.github.io/ccna-roas-simulator/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)]()
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)]()
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)]()

This project is an interactive Network Simulator focused on demonstrating **Inter-VLAN Routing** using the **Router-on-a-Stick (RoaS)** topology. It was developed as a hands-on study tool for the **Cisco CCNA (200-301)** certification, visually explaining how Layer 2 and Layer 3 devices collaborate to route traffic between isolated broadcast domains.

---

## Project Objective

By default, Layer 2 switches cannot forward traffic between different VLANs. To overcome this, traffic must be routed through a Layer 3 device. The Router-on-a-Stick method utilizes a single physical router interface configured with multiple logical subinterfaces, communicating over an 802.1Q Trunk link.

The core learning objective of this simulator is to visually demonstrate:
1. **Local Switching (Layer 2):** How frames are handled when source and destination are in the same VLAN.
2. **Inter-VLAN Routing (Layer 3):** The process of a host sending traffic to its Default Gateway, the switch tagging the frame up the trunk, the router processing the subinterfaces, and the frame being routed back down to the destination VLAN.

---

## Features

* **Dynamic Path Evaluation:** The simulator intelligently evaluates the source and destination IP addresses and VLAN tags. It automatically decides whether to perform a simple Layer 2 MAC forwarding or a complex Layer 3 routing operation.
* **Visual 802.1Q Tagging:** Watch as the switch attaches a colored VLAN tag to the frame as it enters the trunk, and how the router strips and replaces this tag when routing between subinterfaces.
* **Traffic Operations Console:** A real-time, terminal-style log that explains the routing logic step-by-step, including ingress/egress events, default gateway targeting, and tagging processes.
* **Hacker/Terminal UI:** A customized, dark-themed "Matrix" style interface using native CSS properties, SVG dynamic cables, and glowing neon accents for a premium engineering aesthetic.
* **Zero Dependencies:** Built entirely with Vanilla JavaScript, HTML5, and CSS3. No frameworks, no external libraries.

---

## How to Run the Project

Since this is a front-end only application, running it is incredibly simple.

### Option 1: Live Demo (Recommended)
**[Access the Online Simulator Here](https://fe-katopesla.github.io/ccna-roas-simulator/)**


### Option 2: Run Locally
1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/fe-katopesla/ccna-roas-simulator.git](https://github.com/fe-katopesla/ccna-roas-simulator.git)
      ```
2. Navigate to the project directory:
  ```bash
  cd ccna-roas-simulator
  ```
3. Open the index.html file in your favorite web browser.

*This project has been created as part of the 42 curriculum by <hael-hal>.*

# NetPractice

## Description
NetPractice is a general practical exercise designed to introduce the fundamentals of computer networking. The goal of this project is to configure small-scale networks by manually setting up IP addresses, subnet masks, and routing tables to ensure communication between devices.

Through a series of 10 levels, this project helps users understand how devices communicate within and across subnets, the function of routers and gateways, and the logic behind TCP/IP addressing.

## New Concepts Studied
As required by the project subject, the following networking concepts are central to this exercise

### 1. TCP/IP Addressing
The fundamental addressing scheme used for the internet.
* **IP Address:** A unique identifier for a device on a network (e.g., `192.168.1.1`).
* **Network Portion vs. Host Portion:** An IP address is split into two parts; the subnet mask determines which part identifies the network and which identifies the specific device.

### 2. Subnet Mask / CIDR
* **Subnet Mask:** A 32-bit number that masks an IP address and divides the IP address into network address and host address.
* **CIDR (Classless Inter-Domain Routing):** A notation (e.g., `/24`) that indicates how many bits are used for the network prefix. For example, `/24` is equivalent to `255.255.255.0`.

### 3. Default Gateway
A node (usually a router) on a network that serves as an access point to another network. If a device wants to send traffic to an IP address that is **not** in its own subnet, it must send that traffic to the Default Gateway.

### 4. Routers vs. Switches
* **Switch (Layer 2):** Connects devices within the *same* network. It uses MAC addresses (though in this project, we focus on IP logic).
* **Router (Layer 3):** Connects *different* networks together. It uses IP addresses to forward data packets between networks.

### 5. Routing Tables
A data table stored in a router or a network host that lists the routes to particular network destinations. It tells the device: "If you want to reach IP X, send the packet to Interface Y or Gateway Z."

## Instructions

### Installation & Execution
1.  Download the project attachment and extract the files into a local directory.
2.  Open the `index.html` file in a web browser.
    * **Note:** It is strongly recommended to use **Google Chrome** or a Chromium-based browser, as Firefox may block the tool's functionality.
3.  Enter your **intranet login** in the provided field on the welcome screen. This is mandatory for the evaluation system to work correctly.

### Usage
1.  **Solve the Level:** Modify the unshaded fields (IP address, Mask, Gateway/Route) until the network goals described at the top of the page are met .
2.  **Verify:** Click the **[Check again]** button to test your configuration.
3.  **Export:** Once a level is solved, click **[Get my config]** to download the configuration file for that specific level.

## Submission
To submit this project, you must include the exported configuration files for all levels
1.  Complete all **10 levels**.
2.  Export the configuration file for each level using the **[Get my config]** button.
3.  Place the **10 exported files** at the root of your Git repository

## Resources & References

### Documentation & Tools
* [Cisco: IP Addressing and Subnetting for New Users](https://www.cisco.com/c/en/us/support/docs/ip/routing-information-protocol-rip/13788-3.html)
* [Subnetting Practice](https://subnettingpractice.com/) - Tool for practicing mask calculations.
* [Calculatrice IP / CIDR](https://www.calculatrice-ip.com/) - Useful for verifying ranges.

### AI Usage
*Per the project requirements, the use of AI in this project was limited to the following scope

* **Concept Clarification:** AI was used to explain the difference between specific subnet masks and how routing tables prioritize paths.
* **Error Log Analysis:** AI assisted in interpreting the "destination does not match any route" error logs provided by the training interface.

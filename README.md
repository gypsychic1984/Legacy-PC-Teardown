# Legacy-PC-Teardown
## Operation Butt Naked
### *One HP Pavilion. Zero Components Left Behind.*
This project documents the complete teardown of a legacy HP Pavilion desktop computer. The goal was to gain hands-on experience identifying computer hardware, understanding how components connect to the motherboard, safely removing components, and examining the physical construction of a desktop PC.
Rather than simply studying hardware diagrams, I disassembled the system component by component from RAM, storage, and the power supply to the CPU, cooling system, motherboard, and front I/O assembly until only the chassis remained.
## Project Objectives
- Practice ESD-safe hardware handling
- Identify major desktop computer components
- Identify common power and data connections
- Understand how components physically interface with the motherboard
- Practice complete PC disassembly
- Document observations and troubleshooting encountered during the teardown
- Apply lessons learned to my upcoming custom PC build **Project Athena**
## Starting Point
The system arrived as a complete legacy HP Pavilion desktop. Before removing components, I documented the internal layout and existing condition of the machine.
![Initail view inside the HP Pavilion](images/1st%20Look%20inside%20PC%20Case.jpg)
## Component 1: RAM
### Random Access Memory (RAM)
The first major component removed was the system memory. Before removal, I identified the RAM modules installed in the motherboard's DIMM slots.
**What I learned:**
- RAM provides temporary working memory for the operating system and applications
- DIMM stands for **Dual Inline Memory Module**.
- RAM modules are installed directly into DIMM slots on the motherboard.
- Retaining clips on the DIMM slots secure the modules in place.
- The notch in a RAM module helps ensure that it is installed in the correct orientation.
### Removal
I released the retaining clips and carefully removed the RAM modules by handling them by their edges to avoid touching the electrical contacts.
![RAM modules installed in motherboard DIMM slots](images/Located%20RAM.jpg)
### Installed Memory
The system contained two Hynix 4 GB DDR3 DIMMs, providing 8 GB of total installed memory.
- **Manufacturer:** Hynix
- **Capacity:** 4 GB per module
- **Total Memory:** 8 GB
- **Module Type:** DDR3
- **Module Rating:** PC3-10600U
- **Part Number:** HMT351U6BFR8C-H9
![RAM removed with specificaitons](images/RAM%20removed%20with%20Specs.jpg)

## Component 2: Hard Drive
### Hard Disk Drive (HDD)
 The system used a traditional hard disk drive for long-term data storage. Unlike RAM, which stores data temporarily while the computer is operating, the hard drive provides non-volatile storage and retains data when the computer is powered off.
**What I learned:**
- HDD stands for **Hard Disk Drive**.
- The drive stores the operating system, applications, and user files.
- The drive uses the **SATA (Serial ATA)** interface.
- SATA uses separate connections for data and power.
- The SATA data cable connects the hard drive to the motherboard.
- The SATA power cable connects the hard drive to the power supply.
## Connections and Removal
Before removing the drive, I identified and disconnected its SATA data and power connections. The hard drive was mounted inside a removable drive cage, which had to be released from the chassis before the drive could be removed.

### SATA Connections
![Hard drive SATA data and power connections](images/Hard%20Drive%20SATA%20connections.jpg)

### Drive Cage
![Hard drive mounted in drive cage](images/Hard%20Drive%20Cage.jpg)

### Hard Drive Removed
![Hard drive removed from the system](images/Hard%20Drive%20Removed.jpg)

## Component 3: Power Supply Unit
### Power Supply Unit (PSU)
The power supply unit converts AC Power from the wall outlet into the DC power that the computer's internal components can use. This HP Pavilion used a 300-Watt power supply with permanently attached cables.
**What I learned:**
- PSU stands for **Power Supply Unit**.
- The PSU converts **AC (Alternating Current)** into  **DC (Direct Current)**.
- The PSU distributes power to the motherboard, CPU, storage drives, optical drive, and other components.
- The large 24-pin ATX connector provides the motherboard's main power connection.
- The CPU uses a separate motherboard power connection.
- SATA devices use SATA power connections from the PSU.
- The system used a **non-modular PSU**, meaning its cables are permanently attached to the power supply.
### PSU Specifications
The original HP Power supply was rated for a maximum DC output of **300 watts**.
- **Manufacturer:** Lite-On
- **Maximum Output:** 300 W
- **HP Part Number:** 585008-001
- **Design:** Non-modular
### Removal and Troubleshooting
Before removing the PSU, I traced its wiring and disconnected each power connection from the motherboard and installed devices.

After removing the PSU mounting screws, the power supply still would not release from the chassis. Rather than forcing the component, I inspected the mounting area and discovered a small metal retention tab. Moving the tab slightly released the PSU and allowed it to be removed safely.
**Troubleshooting takeaway:** If all visible fasteners have been removed but a component still will not move, stop and inspect for retaining clips, tabs, rails, or other mounting mechanisms before applying additional force.
### PSU Connections
![PSU Connections](images/PSU%20Harness%20disconnected.jpg)
### Power Supply Housing
![Power Supply Housing](images/Power%20Supply%20Housing.jpg)
### PSU Specifications
![PSU specificaitons label](images/PSU%20Specs.jpg)
### Retention Tab
![PSU retention tab](images/Tab%20Holding%20PSU%20into%20place.jpg)
**Troubleshooting takeaway:** If all visible fasteners have been removed but a component still will not move, stop and inspect for retaining clips, tabs, rails, or other mounting mechanisms before applying additional force.

## Component 4: CPU & Cooling System
### Central Processing Unit (CPU)
The CPU performs the primary processing and instruction execution for the computer. This system contained an Intel Core i5-2400 processor.
**What I learned:**
- CPU stands for **Central Processing Unit**.
- The CPU is installed into a socket on the motherboard.
- This processor uses an **LGA (Land Grid Array)** socket design.
- With LGA, the CPU has flat electrical contact pads while the delicate contact pins are located inside the motherboard socket
- The CPU must be correctly aligned and lowered into the socket without force.
- A retention mechanism secures the CPU in the socket.
### CPU Cooling System
The CPU cooler consisted of a fan and a metal heatsink mounted directly above the processor.
**Cooling path:**

CPU → Thermal Paste → Heatsink → Fan → Airflow

Thermal paste fills microscopic imperfections between the CPU's heat spreader and the heatsink, improving heat transfer between the two surfaces.
### Removal
I disconnected the CPU fan from the motherboard and loosened the four spring-loaded heatsink mounting screws gradually in a diagonal pattern. After releasing the thermal-paste bond, I removed the cooler and exposed the CPU.

The CPU retention mechanism was then released, allowing the processor to be carefully lifted from the socket by its edges without touching the electrical contacts.
### CPU Cooler Identified
![CPU Cooler](images/Identified%20the%20CPU%20Cooler.jpg)
### CPU Cooler Connections
![CPU Cooler Connections](images/CPU%20Cooler%20Connections.jpg)
### CPU Cooler Screws Identified
![CPU Cooler screws identified](images/Identifying%20CPU%20Cooler%20Screws.jpg)
### CPU Cooler Removed
![CPU Cooler Removed](images/CPU%20Cooler%20Removed.jpg)
### CPU Identified
![CPU Removed](images/CPU%20Front%20Removed.jpg)
### CPU Contact Pads
![CPU Contact Pads](images/CPU%20Removed%20Back.jpg)
### LGA Motherboard Socket
![LGA motherboard empty](images/Motherboard%20after%20CPU%20removed.jpg)

## Component 5: Wi-Fi Card
### Wireless Network Adapter
The system included an internal Wi-Fi card that provided wireless network connectivity. The card was installed directly onto the motherboard and connected to an antenna lead.
**What I learned:**
- A Wi-Fi adapter allows the computer to communicate with a wireless network.
- The adapter connects to the motherboard through an expansion interface.
- A small coaxial antenna cable connects to the Wi-Fi card using a snap-on connector.
- The antenna improves the card's ability to transmit and receive wireless signals.
- Small internal components and antenna connectors require careful handling during removal.
### Removal
I disconnected the antenna lead from the Wi-Fi card, removed its retaining screw, and carefully removed the card from its motherboard connector.

Removing the card also exposed significant dust accumulation underneath it, demonstrating that dust can collect in areas that are not visible during normal computer maintenance.
### Wi-Fi Card Identified
![WiFi Card Identified](images/WiFi%20Card%20Identified.jpg)
### Wi-Fi Card Specifications

The removed wireless adapter was identified from its component label:

- **Model:** RT5390
- **Board/Model Marking:** WMIR-280GN
- **HP Part Number:** 638403-001
- **Interface:** Internal wireless network adapter
- **Antenna Connection:** Snap-on coaxial antenna connector

### Wi-Fi Card Removed
![WiFi Card Removed](images/WiFi%20Card%20Removed.jpg)
## Component 6: Motherboard
### System Motherboard
The motherboard is the main printed circuit board (PCB) of the computer. It provides the electrical and communication pathways that allow the CPU, RAM, storage, expansion devices, power supply, and external peripherals to work together.

During the teardown, removing the surrounding components gradually exposed the motherboard and made it easier to understand how the computer's hardware connects as one complete system.

**What I identified:**

- CPU socket and retention mechanism
- DIMM slots for system memory
- PCIe expansion slots
- SATA ports for storage devices
- Main motherboard power connector
- CPU power connector
- CMOS battery
- Internal fan and front-panel headers
- Rear I/O ports
- Motherboard chipset and heatsink
### Motherboard Before Removal
![Motherboard after all connections removed](images/Motherboard%20after%20all%20connections%20removed.jpg)
### Motherboard Connections and Interfaces
Examining the motherboard after the major components were removed made it easier to identify the different slots, ports, sockets, and headers and understand what each one connects to.
#### DIMM Slots
The motherboard contains DIMM slots for installing system RAM. The retaining clips secure each memory module, while the keyed notch helps prevent incorrect installation.
#### PCIe Expansion Slots
PCIe slots allow expansion cards to be added to the computer. Depending on the system and slot size, these can support devices such as graphics cards, network adapters, sound cards, and other expansion hardware.
#### SATA Ports
The motherboard's SATA ports provide data connections for storage and optical devices. During the teardown, I traced the SATA data cables from the hard drive and DVD drive back to these motherboard ports.
 #### Power Connections
 The motherboard receives power from the PSU through its main motherboard power connector. A separate CPU power connection supplies power to the processor's voltage-regulation circuitry.
 #### CMOS Battery
 The coin-cell battery provides backup power for firmware-related settings and the system's real-time clock while the computer is disconnected from external power.
 #### Internal Headers
 Smaller motherboard headers provide connections for components such as cooling fans, front-panel controls, indicator LEDs, USB ports, and other chassis features.
 #### Rear I/O
 The rear I/O section provides the computer's external connections. This system included connections for USB, Ethernet networking, audio, and video output.
 ### Motherboard Interfaces
 ![Motherboards interfaces and rear I/O](images/I_O%20Panel%20Identified.jpg)
 ### Rear I/O Assembly Removed
 ![Motherboards I/O assembly removed](images/I_O%20Assembly%20Removed%20with%20Specs.jpg)
 ### Motherboard Removal
 With the major components and motherboard connections removed, I inspected the board for its mounting points before attempting to lift it from the chassis.

I identified **eight motherboard mounting screws**: seven positioned around the outer perimeter and one additional screw near the center of the board.

After removing the screws, I carefully checked that no cables or connectors were still attached before moving the motherboard.

**What I learned:**

- Motherboards are secured to the chassis using screws and raised mounting points called **standoffs**.
- Standoffs keep the underside of the motherboard from making direct contact with the metal chassis.
- The rear I/O ports must clear the chassis opening before the motherboard can be completely removed.
- A motherboard should never be forced from the case if it does not move freely.
- Before lifting the board, cables, mounting screws, retaining points, and the rear I/O area should all be checked again.
### Motherboard Removed From Chassis
Once all mounting points were released and the rear I/O connections were clear of the chassis, I carefully removed the motherboard and placed it on my ESD-safe work surface.
![Motherboard Removed](images/Motherboard%20removed.jpg)
### Why Standoffs Matter
The motherboard does not sit directly against the metal computer case. Standoffs create a small physical gap between the motherboard and chassis while also providing secure mounting locations.

Without proper standoff placement, conductive areas on the underside of a motherboard could contact the metal chassis and potentially cause an electrical short.
### Chassis After Motherboard Removal
![Chassis after Motherboard removed](images/Underneath%20Motherboard%20Cleanest%20so%20far.jpg)

## Component 7: DVD Optical Drive
### DVD/CD Rewritable Drive
The system included an internal DVD/CD rewritable optical drive used to read and write optical media. During the teardown, I identified both the drive's data and power connections before removing it from the chassis.

**What I learned:**

- DVD stands for **Digital Versatile Disc**.
- CD stands for **Compact Disc**.
- The optical drive uses a SATA data connection to communicate with the motherboard.
- The drive requires a separate power connection from the PSU.
- SATA data and SATA power connectors have different widths and functions.
- The drive was mechanically secured inside the chassis and had to be released before it could slide out.

### Connections and Removal

Before removing the optical drive, I disconnected its SATA data and power connections. Once the connections were clear and the drive was released from its mounting position, I slid the drive out of the chassis.
### DVD Drive Identified
![DVD Burner_Player Identified Casing](images/DVD%20Burner_Player%20Identified%20casing.jpg)
#### SATA Connections
![DVD Burner_Player SATA Connections](images/DVD%20Burner_Player%20SATA%20Connections.jpg)
### Power Connection
![DVD Power Supply Identified](images/DVD%20Power%20Supply%20Identified.jpg)
### Optical Drive Specifications
The removed optical drive was identified from its component label:

- **Type:** DVD/CD Rewritable Drive
- **Model:** AD-7251H
- **HP Part Number:** 657958-001
- **HP Spare Part Number:** 615646-001
- **Manufactured:** July 2011
![DVD Burner_Player Removed_Specs](images/DVD%20Burner_Player%20Removed_Specs.jpg)
## Component 8: Front I/O & Card Reader
### Front Input/Output (I/O) Assembly
The front I/O assembly provides convenient external connections at the front of the computer. Unlike the rear I/O ports that were integrated with the motherboard, this assembly was mounted to the chassis and connected back to the motherboard with internal cables.

**What I learned:**

- I/O stands for **Input/Output**.
- External ports provide an interface between the user, peripheral devices, and the computer.
- Front-panel ports connect to internal motherboard headers through cables.
- USB ports can carry both data and electrical power.
- Audio connections provide input and output paths for devices such as microphones, headphones, and speakers.
- Front-panel assemblies may use tabs, rails, clips, or screws in addition to electrical connections.

### Removal

I traced and disconnected the front I/O assembly cables before removing the assembly from the chassis. After removing its retaining screw, the assembly initially remained attached. I discovered that it was also secured by the chassis mounting design and released it by sliding the assembly slightly before removing it completely.

**Troubleshooting takeaway:** A component that remains secured after its visible screw is removed may also use tabs, slots, rails, or other mechanical retention features.
### Front I/O Assembly Removed
![Front I/O Assembly Removed with Specs](images/I_O%20Assembly%20Removed%20with%20Specs.jpg)
### Card Reader Identified
![Card Reader Identified](images/Card%20Reader%20Assembly.jpg)
The system also contained an internal multi-format card reader mounted in the front of the chassis. The reader allowed removable flash-memory cards to interface with the computer.
Removing the card reader provided another example of how front-mounted devices combine electrical connections with mechanical mounting hardware.
### Card Reader Removed
![Card Reader Removed](images/Card%20Reader%20Removed%20with%20Specs.jpg)
## Component 9: Chassis Fan & Airflow
### Chassis Cooling Fan
The chassis fan helps control the internal temperature of the computer by moving air through the case. This airflow helps remove heat generated by components such as the CPU, motherboard, power supply, and storage devices.

**What I learned:**

- Case fans create airflow through the computer chassis.
- Cool air enters the case while warmer air is exhausted.
- Proper airflow helps prevent excessive component temperatures.
- Dust accumulation can restrict airflow and reduce cooling efficiency.
- Fan blades and ventilation openings require periodic cleaning as part of preventive maintenance.
- Cooling problems are not always caused by failed hardware; restricted airflow can also contribute to overheating.

### Removal
I disconnected the chassis fan's power cable from the motherboard and removed the fan from the rear of the case.
Once removed, the amount of dust accumulated on the fan blades and housing was clearly visible.
### Chassis Fan Removed
![Chassis Fan Removed](images/Case%20Chassis%20Fan%20Removed.jpg)
### Preventive Maintenance Observation
The fan showed heavy dust accumulation across the blades and surrounding frame. Similar dust buildup was found throughout the computer, including around the CPU cooler, motherboard, expansion components, and ventilation areas.

This teardown demonstrated why routine internal cleaning is important. Dust can obstruct ventilation, reduce heat-transfer efficiency, and force cooling fans to work harder to maintain acceptable temperatures.

**Maintenance takeaway:** Keeping vents, heatsinks, fans, and airflow paths clean is an important part of maintaining reliable computer hardware.
# Final Teardown: Operation Butt Naked
## One HP Pavilion. Zero Components Left Behind
The teardown was completed with the major internal hardware removed from the HP Pavilion chassis. What began as a complete legacy desktop was reduced component by component until the internal chassis was essentially bare.

Throughout the project, I did more than remove parts. I identified components, traced power and data connections, examined mounting systems, documented specifications, practiced ESD-safe handling, and worked through several unexpected mechanical obstacles without forcing the hardware.

### Components Removed and Examined

- RAM (Random Access Memory)
- HDD (Hard Disk Drive)
- PSU (Power Supply Unit)
- CPU (Central Processing Unit)
- CPU cooling system
- Wi-Fi network adapter
- Motherboard
- DVD/CD optical drive
- Front I/O assembly
- Multi-format card reader
- Chassis cooling fan

### Final Chassis

After the final components were removed, only the chassis and a small amount of integrated front-panel wiring remained.
### HP Chassis Case Specs
![HP Empty Case Specs](images/HP%20Case%20Empty%20Specs.jpg)
### HP Empty Chassis Front without Bezel
![HP Case Empty Front without Bezel](images/HP%20Case%20Empty%201.jpg)
### HP Empty Chassis Interior
![HP Case Gutted](images/HP%20Case%20Empty%202.jpg)
### HP Empty Chassis Rear View
![HP Case Rear View Empty](images/HP%20Case%20Empty%20Rear%20View.jpg)
## Key Lessons Learned
This project helped turn computer hardware concepts that I had previously studied into physical, hands-on experience.

- Hardware diagrams became easier to understand after physically locating the components.
- Power connections and data connections serve different purposes and can often be identified by tracing where their cables terminate.
- Components should never be forced during removal. Hidden tabs, clips, rails, and retention mechanisms should be investigated first.
- ESD precautions are important when handling exposed electronic components.
- Motherboard standoffs prevent the board from resting directly against the metal chassis.
- Heavy dust accumulation can interfere with airflow and cooling and demonstrates the importance of preventive maintenance.
- Component labels provide valuable information such as model numbers, part numbers, capacity, power ratings, and manufacturing information.
- Photographing and documenting a teardown creates a useful technical record and reinforces hardware identification skills.

## Applying This to Project Athena

The knowledge gained during this teardown will be applied directly to my custom PC build, **Project Athena**.

By disassembling a complete desktop computer first, I gained practical experience with motherboard mounting, CPU installation and retention, RAM placement, storage connections, power distribution, cooling, cable routing, expansion interfaces, and chassis construction.

Project Athena will reverse the process demonstrated in this repository: instead of beginning with a complete computer and reducing it to an empty chassis, I will begin with individual modern components and assemble them into a complete working system.

**Legacy-PC-Teardown taught me how a computer comes apart. Project Athena will demonstrate that I understand how one goes together.**


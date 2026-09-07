# Legacy-PC-Teardown
## Operation Butt Naked
### *One HP Pavilion. Zero Components Left Behind.*
This project documents the complete teardown of a legacy HP Pavilion desktop computer. The goal was to gain hands-on experience identifying computer hardware, understanding how components connect to the motherboard, safely removing components, and examining the physical construction of a desktop PC.
Rather than simply studying hardware diagrams, I disassembled the system component by component from RAM, storage, and the power supply to the CPU, cooling system, motherboard, and front I/O assembly until only the chassis remained.
## Project Objectives
- Practice ESD-Safe hardware handling
- Identify major desktop computer components
- Identify common power and data connections
- Understand how components physically interface with the motherboard
- Practice complete PC disassembly
- Document obserbations and troubleshooting encounterd during the teardown
- Apply lessons learned to my upcoming custom PC build **Project Athena**
## Starting Point
The system arrived as a complete legacy HP Pavilion desktop, Before removing components, I documented the internal layout and existing condition of the machine.
![Initail view inside the HP Pavilion](images/1st%20Look%20inside%20PC%20Case.jpg)
## Component 1: RAM
### Random Access Memory (RAM)
The first major component removed was the system memory. Before removal, I identified the RAM modules installed in the motherboard's DIMM slots.
**What I learned:**
- RAM provides temporary working memory for the operating system and applications
- DIMM stands for **Dual Inline Memory Module**.
- RAM modules are installed directly into DIMM slots on the motherboard.
- Retaining clips on the DIMM slots secure the modules in place.
- The notch in a RAM module helps ensure that it is installed in the correct oreintation.
### Removal
I realeased the retaining clips and carefully removed the RAM modules by handling them by their edges to avoid touching the electrical contacts.
![RAM modules installed in motherboard DIMM slots](images/Located%20RAM.jpg)
### Installed Memory
The system contained two Hynix 4 GB DDR3 DIMMs, providing 8 GB of total installed memory.
- **Manufacturer:** Hynix
- **Capacity:** 4GB per module
- **Total Memory:** 8 GB
- **Module Type:** DDR3
- **Module Rating:** PC3-10600U
- **Part Number:** DHMT351U6BFR8C-H9
![RAM removed with specificaitons](images/RAM%20removed%20with%20Specs.jpg)

## Component 2: Hard Drive
### Hard Disk Drive (HDD)
 The system used a traditional hard disk drive for long-term data storage. Unlike RAM, which stores data temporarily while the computer is operating, the hard drive provides non volatile storage and retains data when the computer is powered off.
**What I leared:**
- HDD stands for **Hard Disk Drive**.
- The drive stores the operating system, applications, and user files.
- The drive uses the **SATA (Serial ATA)** interface.
- SATA uses separate connections for data and power.
- The SATA data cable connects the hard drive to the motherboard.
- The SATA power cable connects the hard drive to the power supply.
## Connections and Removal
Before removing the drive, I identified and disconnected it's SATA data and power connections. The hard drive was mounted inside a removable drive cage, which had to be released from the chassis before the drive could be removed.

### SATA Connections
![Hard drive SATA data and power connections](images/Hard%20Drive%20SATA%20connections.jpg)

### Drive Cage
![Hard drive mounted in drive cage](images/Hard%20Drive%20Cage.jpg)

### Hard Drive Removed
![Hard drive removed from the system](images/Hard%20Drive%20Removed.jpg)




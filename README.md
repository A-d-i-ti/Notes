# understanding the system 
## Desktop has 3 major components :
1.Computation 
2.Storage
3.Networking 
### COMPUTATION :
Central Proccessing Unit (CPU) is responsible for computation.
It works on ISA (Instruction Set Architecture) .
+ ISA : The processor is the brain of any computer, and it is constantly evolving to improve efficiency.
A processor’s design determines how many instructions it can do and how fast and efficiently it can do them. 
- CISC (Complex Instruction Set Computer"),RISC(Reduced Instruction Set Computer), RISC-V(open source ), and ARM are terms used in processor design
    to denote a type of processor using a specific type of instruction set architecture (ISA)
- CISC based proccessors - Intel (X-86) ,AMD
- RISC processors based ARM (ISA) - APPLE
### some computer system architecture :
- VON NEUMMAN
- HARVARD ARCHITECTURE
![difference bwt the above](https://fabacademy.org/2020/labs/vigyanashram/students/snehal-gawali/assignment8/images/3.jpg)
### NUMA :Non-uniform memory access (NUMA)
- is a computer memory design used in multiprocessing, where the memory access time depends on the memory location relative to the processor.
 Under NUMA, a processor can access its own local memory faster than non-local memory (memory local to another processor or memory shared between processors).
![numa vs uma ](https://cse.buffalo.edu/faculty/miller/Talks_HTML/Erice-Parallel/sld015.gif)
### NETWORKING :
1.INTRANET(LAN)  2.INTERNET (WAN)
- **The Open Systems Interconnection (OSI)** model describes seven layers that computer systems use to communicate over a network.
![osi](https://www.imperva.com/learn/wp-content/uploads/sites/13/2020/02/OSI-7-layers.jpg)
- L7 : app/protocol
- L6:
- L5: Cryptography
- L4 :Port number(16 bits) ,Transport layer security(TLS)tunnel used for VPN(Virtual Private Network)
- L3 :IP address (32 bits)
- L2 :MAC Address 
- L1 :0 and 1 
- **L7+L6+L5 ---> TCP/IP**

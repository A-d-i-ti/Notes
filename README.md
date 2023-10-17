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
- L2 :MAC Address /internet
- L1 :0 and 1 
- **L7+L6+L5 ---> TCP/IP**
-**IP ADDRESS**- THREE MAIN TYPES :
- PRIVATE IP - majorly LAN (10.____ , 172.16._____ , 192.68.____)
- PUBLIC IP - can be accessed by anyone on the internet
- LOCAL IP - local host that is our own system (127.0.____)
-**COMMUNICATION** : wired(optical fiber,) and wireless (wifi ,EMWaves )
### STORAGE :
1.KERNAL SPACE and User space :
![kernal and user space ](https://qph.cf2.quoracdn.net/main-qimg-150cb90563a482ea7d2198964beee8fb-lq)
+ C,C++ ,RUST --->programing languages for writing kernal space :
- BARE METAL = FRESH SERVER 
### HYPERVISOR :
A hypervisor, also known as a virtual machine monitor or VMM, is software that creates and runs virtual machines (VMs).
A hypervisor allows one host computer to support multiple guest VMs by virtually sharing its resources, such as memory and processing. 
- 2 main hypervisor ----> “Type 1” eg:kvm (or “bare metal”) and “Type 2” eg:vmware workstation, (or “hosted”).
### FPGA(Field Programmable Gate Array.)
An FPGA is an IC (Integrated Circuit) programmed for performing customized operations for a specified application.
**silicon chip** tiwan is the largest producer.
## SOME KEYWORDS :
1. **Computer simulation** -the use of a computer to represent the dynamic responses of one system by the behavior of another system modeled after it.
2. **Cryptography** - the process of hiding or coding information so that only the person a message was intended for can read it. 2types -- classical and Post Quantum 
3. **Socket** - IP (layer 3)+PORT NUMBER (Layer 4)
4.**PORT NUMBER**- used to access particular protocol .eg: http- 80 ,https-443 ,ftp :20 or 21,telnet -23 ,SSH(secure shell) -22 , SMTP -25
5. Every program in the main memory is calleda **PROCCESS**.
6. **HTTPS**- S stands for SSL i.e.**secure socket(ip+port no) layer** is a certificate (X.509) provided by a certified Authority eg.Godaddy
7. **FCFS**-First come first serve
8. **ROUND ROBIN**- algorithm that works on FCFS .runs 2-3 process together ,equal time to all process --> called **FAIR ALGORITHM**
9. **PING** -hitting a website to check the internet eg: ping 4.2.2.2 (to check internet)
                                                         ping 8.8.8.8 (google server ping)
10.**APIPA stands for Automatic Private IP Addressing-** It is a feature or characteristic in operating systems (eg. Windows) which enables computers to self-configure an IP address and subnet mask automatically when their **DHCP**(Dynamic Host Configuration Protocol) server isn't reachable
11. **NAT (network address translation)**-translates Private IP to PUBLIC IP and vice versa .
12. **Switch**- layer-2 of OSI ,a device in a computer network that connects other devices together.
13. **Router**- layer-3 of OSI ,a device that connects two or more packet-switched networks or subnetworks.
14. **SERVER**-  a computer or system that provides resources, data, services, or programs to other computers, known as clients, over a network.eg.Apache
15. **PROXY SERVER**- a system or router that provides a gateway between users and the internet. EG.Apache,nginx
16. 

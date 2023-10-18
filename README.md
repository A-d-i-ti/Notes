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
### CNI (CONTAINER NETWork interface):
CNI is a Cloud Native Computing Foundation project, consists of a specification and libraries for writing plugins to configure network interfaces in Linux containers, along with a number of plugins.
-plug-in is a piece of software that adds new features or extends functionality on an existing application.
Network models in cni :
- Encapsulated Network :
  ![ESY EXPLAINATION ](https://ranchermanager.docs.rancher.com/assets/images/encapsulated-network-0c75db46568d5b2636dad4a8c28d3cc4.png)
  CNI network providers using this network modEL - Flannel, Canal, Weave, and Cilium.
  + FLANNEL-Flannel is a Container Network Interface (CNI) plug-in that you can use to create a virtual network for containers based on Virtual Private Cloud (VPC)
- Unencapsulated Network:
  ![LIST ](https://ranchermanager.docs.rancher.com/assets/images/unencapsulated-network-b87922f280aa17322e6485b81855dd4a.png)
  **ETCD-**is an open source, distributed, consistent key-value store for shared configuration, service discovery, and scheduler coordination of distributed systems or clusters of machines
  standard system for container orchestration.
  CNI network providers using this network model include Calico and Cilium.
   + **Calico** uses a pure, unencapsulated IP network fabric and policy engine to provide networking for your Kubernetes workloads.
      Workloads are able to communicate over both cloud infrastructure and on-prem using BGP(Border Gateway Protocol ).
**CNI Providers :**
Canal is a CNI network provider that gives you the best of Flannel and Calico. It allows users to easily deploy Calico and Flannel networking together as a unified networking solution
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
15. **PROXY SERVER**- retrives data on the internet on behalf of a user
     -hides your public IP address . EG.Apache,nginx
16. **system design** : the process of defining the architecture, interfaces, and data for a system that satisfies specific requirements.
    ![design](https://media.geeksforgeeks.org/wp-content/uploads/20221117170254/OBJECTIVESOFSYSTEMDESIGN.png)
17. **HUGE PAGES**-Memory is managed in blocks known as pages.CPUs have a built-in memory management unit that contains a list of these pages, with each page referenced through a page table entry.
18. **CEPF**-Ceph is an open source storage platform that is designed to allow object, block, and file storage from a single system.
19. **API -** application programming interface — a software intermediary that allows two applications to talk to each other.
20. **REST API **- A REST API is an API that conforms to the design principles of the REST, or representational state transfer architectural style.
21. **BROWN FIELD**-(monolithic)Brownfield software development refers to the development and deployment of a new software system in the presence of existing or legacy software systems.
22. **Green field**-(microservices )developing a system for a totally new environment, without concern for integrating with other systems, especially not legacy systems.
23. **HA**- High availability
24. **SSO**-CONCEPT OF WEB 2.0 ,**single sign on** with only gmail login into youtube ,google
25. WEB 3.0- DECENTRALISATION of information ,used case -identity authentication
26. **LLM model**- A large language model (LLM) is a deep learning algorithm that can perform a variety of natural language processing (NLP) tasks. eg.chatgpt
27. -LLM uses vector database .
28. **Cloud-native development** is just that—an approach to building and updating apps quickly, while improving quality and reducing risk
29. **Border Gateway Protocol (BGP)** refers to a gateway protocol that enables the internet to exchange routing information between autonomous systems (AS)
30. Ingress/Egress Policies: This feature allows you to manage routing control for both Kubernetes and non-Kubernetes communications.
31. Infrastructure as code (IaC) - uses DevOps methodology and versioning with a descriptive model to define and deploy infrastructure, such as networks, virtual machines, load balancers, and connection topologies.
32. DEVOPS-DevOps is a combination of software development (dev) and operations (ops)
33. KUBERNETICS (K8S) - container orchestration technology,
34. POD - Containers are called PODs in k8s
35. RANCHER - allows users to manage multiple Kubernetes' clusters more efficiently.
36. Terraform - is an IAC tool, used primarily by DevOps teams to automate various infrastructure tasks.
37.** Hashing **- technique or process of mapping keys, and values into the hash table by using a hash function.
38. MERN - stands for MongoDB, Express, React, Node, after the four key technologies that make up the stack. MongoDB — document database. Express(.js) — Node.js web framework. React(.js) — a client-side JavaScript framework.
39. BLOCKCHain : stores the transactions
40. blockchain uses Datatbases .
41. **Homomorphic encryption** is a form of encryption that allows computations to be performed on encrypted data without first having to decrypt it. anonimity and confidentiality .

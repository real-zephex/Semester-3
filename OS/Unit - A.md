## Operating System
An operating system is a core software component that acts as an intermediary between a computer's hardware, application programs, and users. It divides the overall computer system into four main parts: 
1. The hardware
2. The OS itself
3. Applications programs
4. The users

#### Features of Operating System
1. Hiding Hardware Complexity
	- The OS conceals the low-level hardware details (e.g.: CPU, memory, I/O devices), allowing programs to interact with the hardware in simple, abstracted ways.
2. Resource Management and Allocation
	- It serves as a resource allocator, efficiently managing and distributing system resources (like processing power and storage) among applications to create an optimal computing environment.
3. Enabling Useful Work
	- The OS provides a structured environment that facilitates the creation and execution of useful software by applications.

###### User View
- The user view refers to how the end-user perceives and interacts with a computer system.
- It is one side of the "abstract view of system components", where the OS  acts as a bridge between the user/application layer and hardware. 
- The primary goal is to improve user's productivity which it achieves by providing applications such as word processors, browsers an environment to run smoothly, abstracting the complexities of managing low-level hardware.
- ![[Pasted image 20250922031944.png]]

###### System View
- It refers to the perspective of the operating system itself, focusing on how it interacts with and manages the underlying computer hardware to ensure efficient, fair, and reliable approach.
- The system goal is to optimise the overall performance and resource allocation without bias. 
- It's also responsible for proactive error prevention for issues such as conflicting resource requests or improper operations.

###### Kernel
- The **kernel** is the core of the operating system, acting as the foundational software layer that directly interacts with hardware while managing system resources. 
- It is the `heart` of the OS, providing essential services to applications and users without being an application itself. 
- ![[Gemini_Generated_Image_2x2y612x2y612x2y(1).png]]
- Key functions of the kernel: resource management, hardware abstraction, process management, memory management, system calls, etc.

#### Resource Management in OS
- An operating system is a **resource manager**. 
- The system's CPU, memory space, file-storage space, and I/O devices are among the resources that the operating system must manage.

###### Process Management
- A process is a program in execution, serving as the fundamental unit of work in a system. Unlike a static program, a process is an active entity.
- The OS allocates CPU, memory, I/O devices, and other resources to processes to accomplish their tasks. 
- The OS is responsible for creating and deleting both user processes and system processes. Multiple processes can stem from the same program, with each having their own execution counters and sequences.
- It also handles issues like process coordination and communication, while preventing conflicts such as [^1]`deadlocks`.

###### Memory Management
- Memory Management is a core function of the OS that handles the allocation, tracking, and efficient use of main memory (RAM) which serves as a fast repository for data and instructions shared between CPU and I/O devices.
- It dynamically allocates memory space for programs and deallocates space upon termination, making space available for subsequent tasks to improve overall efficiency.
- The OS decides which processes (or parts thereof) and data to move into and out of memory to balance utilisation and speed.

###### File Management
- File management in the operating system ensures the organized storage, access and control of files.
- The OS abstracts the physical storage details to present a logical view of files, making it easier for users to work with data.
- It manages how files are stored on different types of storage devices (like hard drives or SSDs) and ensures smooth access through directories and permissions.

###### Device Management
- Device management of an operating system handles the communication between the system and its hardware devices, like printers, disks or network interfaces.
- The OS handles the actual transfer of data to and from devices. This includes managing buffers, handling interrupts, and ensuring data integrity.
- When errors occur during device operations (e.g., printer jam, disk error), the OS detects and attempts to handle these errors gracefully, informing the user or application as needed.

###### Protection and Security
- Mechanisms in an operating system are designed to safeguard system resources from unauthorised access or misuse. 
- These mechanisms control which processes or users can access specific resources (such as memory, files, and CPU time) and ensure that only authorised users can perform specific operations.

---

#### Types of Operating System
1. Batch Operating System
2. Multiprogrammed Operating System
3. Time-Shared Operating System
4. Personal Operating System
5. Parallel Operating System
6. Distributed Operating System
7. Real-Time Operating System

###### Batch Operating System
- Jobs having similar requirements are grouped and executed as a group to speed up processing. 
- Users using batch operating system do not interact with the computer directly. 
- A Batch Processing Operating System (BPOS) is designed to handle and process large volumes of data in batches, making it ideal for organisations that require efficient and rapid data processing.

###### Multi-programmed Operating System
- Multi-programming means that more than one program can be active at the same time. 
- The idea of multi-programming is to assign CPUs to other processes while the current processes might not be finished.

###### Time-Shared Operating System
- Time-shared operating system allows multiple users to interact with a computer system simultaneously.
- Time-sharing uses CPU scheduling and multi-programming to allocate a small portion of the CPU to each user.

###### Personal Operating System
- A personal operating system is designed for individual use on personal computers.
- A personal operating system contains various kind of software which aids with productivity and workflow of an individual.
- It offers user-friendly GUI and abstracts all the heavy lifting and provides an easy to use interface to interact with the system.

###### Parallel Operating System
- A parallel operating system are designed to utilize multiple processors to execute tasks simultaneously.
- The idea here is to increase processing speed and make use of better performance to perform complex problems faster. 

###### Distributed Operating System
- A distributed operating system manages a network of independent, physically separate computers or nodes, making them appear as a single, unified system to the user.
- It leads to better fault tolerance as others can take over if one machine fails.
- Users can access  resources on different machines.

###### Real-Time Operating System
- A real-time operating system is a special kind of operating system designed to handle tasks that need to be completed quickly and on time.
- Unlike general purpose operating system, RTOS focuses on doing things in real time.
- An RTOS provides real-time control over hardware resources and utilizes system resources efficiently while maintaining high reliability and responsiveness.

---

#### System Calls
System calls are programmatic interfaces between user applications and the operating system (OS). They provide a controlled mechanism for applications to request services from the kernel, enabling access to hardware without direct manipulation

###### Key characteristics of System Calls
1. **Privileged Operations**: Allow user programs to access hardware/resources managed by the OS. (e.g.: files, memory, processes)
2. **Standardised Interface**: Abstract low-level hardware details, providing a unified API across different systems.
3. **Synchronous**: Blocks execution until the OS completes the request
4. **System-dependent**: Implementation varies across operating system (e.g.: Linux, Windows, MacOS)



[^1]: A **deadlock** is a situation where a set of processes gets permanently stuck because each process is waiting for a resource held by another process, and none of them can proceed.

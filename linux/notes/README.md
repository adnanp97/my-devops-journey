# Linux notes

### Intro to Linux Operating System (OS) and Kernels
---
**What is Linux?**
Linus is an operating systyem. An operating system is software which allows you to interact and send instruction to hardware via a kernel.

**User Interaction:** 
The user interacts with the operating OS. This interaction can be through a graphical user interface (GUI) with windows and icons or a command-line interface (CLI) with text commands.

**Role of the Kernel:** 
The operating system includes the kernel, which is the core part of the OS. The kernel handles critical tasks such as managing hardware resources (CPU, memory, storage) and executing system calls from applications.

**Kernel and Hardware:** 
When the user performs an action, such as opening a file or running an application, the OS translates these actions into requests that the kernel processes. The kernel then communicates with the hardware to complete these tasks.

**Summary:**
User → Interacts with the OS.  
OS → Includes the Kernel.  
Kernel → Handles hardware interactions and executes tasks.  
So, the kernel does the actual work of interacting with the hardware based on the user's commands processed by the operating system. 

My understanding:
A user interacts with an operating system (software e.g. Linux), this operation system has a kernel. When a person interacts with the operating system, the real work is done by the kernel which interacts with the actual hardware. 

**Note: Without an operating system or kernel, you will not be able to interact with the hardware**
- No operating system means there will be not interface to interact with the computer.  
- No kernel means tasks will not get excetued as the kernel is what tells the hardware (like the CPU, memory, and storage) how to work together. Without it, your computer wouldn’t know how to use its parts.

---
### Intro to command line interface (CLI) and shell
---
**What is command line interface (CLI) for?**

- The CLI allows you to interact with OS by typing commands. You can run scripts, exceute commands and manage system effeciently.  
- Your input is a command which is interpreted by the shell and the result is the standard output.  
- Commands are case sensitive.  
- Has 3 attributes which modify their behaviour: '$ Command Options Arguments'.  

**The purpose of a shell:**
To serve as a CLI between the user and the OS. It allows you to interact with the system by typing commands, which the shell interprets and executes.  
There are different shells each with their own benefits and purposes but all have one fundamental purpose; to allow you to communicate with the system.  
**user -> shell -> kernel -> hardware**  

`cat/etc/shells` - prints all shells available on your system.  
`chsh -s /usr/bin/zsh` - change default shell to zsh

**Program and Binaries**
Commands such as ls, grep, echo are small programs which are written in a programming language. 
These programs are compiled into a format the computer can execute called binaries.  
Developer create the program with a specific task e.g. ls.  
Binary: compiled version of prgram that computer can run directly.

**What happens when you run a command**
- Type a command e.g. $ ls
- Shell interprets; understand we want to run the ls program.
- Shell searches for program in certain directories on computer which are listed in the path environment variables.
- Once ls program is found, it runs/executes it and lists the content.

---
Vim stuff [place hold]

DevOps care about Nginx because it helps manage web traffic efficiently. It can serve as a reverse proxy, which means it sits between users and web servers, directing user requests to the right server and improving speed and security.

Example: Imagine Nginx as a receptionist in a busy office. When people (users) walk in (make requests), the receptionist (Nginx) directs them to the correct office (server) without them needing to know exactly where to go. This makes everything run smoothly.
---




### Binary, Octal and String Representation!
---
![Screenshot 2024-09-01 at 14 21 09](https://github.com/user-attachments/assets/2146e65b-92bf-4cc1-93f5-967871a5b17a)
![Screenshot 2024-09-01 at 14 25 52](https://github.com/user-attachments/assets/2dc8797e-716d-4f87-b7c6-76fb080a1086)


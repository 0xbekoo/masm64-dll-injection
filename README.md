## `⚠️` DLL Injection with MASM64 Assembly

This project demonstrates the implementation of DLL Injection using MASM64 Assembly. DLL Injection is a widely used technique to load a dynamic link library (DLL) into the memory space of a target process.

## `🔧` Prerequisites

Before you begin, ensure you have the following tools installed:

- MASM64 (Microsoft Macro Assembler for 64-bit Windows)
- Microsoft Visual Studio (or any IDE supporting MASM64)
- x64dbg or a similar debugger (optional but recommended for debugging purposes)
- Windows 10/11 x64 (The code is tailored for modern Windows OS, and might not work on older versions)

Since the project does not use any function to print the program's status to the screen, you will need to track the results using a debugger tool.

## `⚙️` Required Modifications Before Running the Project
Before running the project, some changes need to be made. Follow the steps below to update the necessary configurations:

- **PID Value:** The PID value is set to 0 by default in the main.asm file. Change this to your target PID value:

```asm
.const 
    ; Make sure you enter the PID
    PID DW 0
```
<br>

- **DLL**: You need to provide the path to the DLL you have prepared for the project:

```asm
.const 
    ...

    ; Make sure you enter the path to your dll
    dllPath db "\path\to\dll",0 
```

Give the path to the DLL to this variable.

## 🚨 Disclaimer
This project has been developed solely for educational purposes. It is intended to demonstrate concepts related to DLL Injection using MASM64 Assembly and is not intended for use in any real-world malicious activities.

Usage in real-world scenarios is at your own risk. The author is not responsible for any damage, misuse, or legal consequences that may arise from using or distributing this project. 

# EXPERIMENT--01-ALP-FOR-8086
Name :HARISHA.S
Roll no :212224230087
Date of experiment : 29/08/2025



## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)


9.	Click on emulate to start emulation 


![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)



10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 


![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)

## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```
## Output  
 <img width="1906" height="1151" alt="ADD" src="https://github.com/user-attachments/assets/8d0e5288-8a67-4b72-8167-5bf0a908b501" />

## Subtraction   of 8 bit numbers  ALP 
 ```MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```
## Output  
<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/b3b7ef7d-8d2b-4f22-9197-0eed08d5ae27" />

## Multiplication alp 
```MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
 ## Output  
<img width="1280" height="799" alt="image" src="https://github.com/user-attachments/assets/85f6b8f0-4db8-4a73-8f6f-e68e32c3e818" />

## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
## Output  
<img width="1882" height="1092" alt="Screenshot 2025-08-29 152133" src="https://github.com/user-attachments/assets/cbc238fe-2f33-4572-b444-b374b25ee64b" />

## LOGICAL OPERATORS
## ADD
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="1902" height="1152" alt="add2 emu" src="https://github.com/user-attachments/assets/21aab44f-8eeb-44bd-8eb8-4b5b8bf705fd" />

## NAND
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```

## OUTPUT
<img width="1894" height="1161" alt="Screenshot 2025-08-29 153522" src="https://github.com/user-attachments/assets/9cbf353d-642c-4646-9928-50e92ac7c610" />

## OR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```

## OUTPUT
<img width="1900" height="1112" alt="Screenshot 2025-08-29 152927" src="https://github.com/user-attachments/assets/5876af54-e728-47b9-90b5-a879d6fd28be" />

## NOR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```

## OUTPUT
<img width="1894" height="1150" alt="Screenshot 2025-08-29 153401" src="https://github.com/user-attachments/assets/0e71382a-2935-4e6c-a571-89a2be7ad0de" />

## NOT
```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT
```

## OUTPUT
<img width="1887" height="1140" alt="Screenshot 2025-08-29 154310" src="https://github.com/user-attachments/assets/3f71550e-6a90-4e9d-8b0d-47c2ab7f6dec" />

## XOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```

## OUTPUT
<img width="1914" height="1151" alt="Screenshot 2025-08-29 154813" src="https://github.com/user-attachments/assets/d6e41b1c-f5a0-4105-bcef-96f3fd3cbdf4" />

## XNOR
```

MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```

## OUTPUT
<img width="1883" height="1185" alt="Screenshot 2025-08-29 154941" src="https://github.com/user-attachments/assets/af022c33-fa64-4d47-969f-42c64540e6bc" />


## Result :
 Successfully write and execute ALP on fundamental arithmetic and logical operations.









## EXPERIMENT--01-ALP-FOR-8086
Name : Vinutha V

Roll no : 212225230306

Date of experiment : 07/11/2026





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

## Addition ALP 
```
Org 100h
Mov ax, [1100h]
Mov bx, [1102h]
Add ax,bx
Mov [1200h],ax
ret
```


## Output  
<img width="1552" height="961" alt="Screenshot 2026-11-18 000041" src="https://github.com/user-attachments/assets/83695ac1-41d8-44f4-8382-b2f70affb6d0" />

 
## Subtraction  ALP 
```
Org 100h
Mov ax,[1100h]
Mov bx,[1102h]
Sub ax, bx
Mov [1200h], ax
ret
```
 
## Output 
<img width="1722" height="975" alt="Screenshot 2026-11-18 000341" src="https://github.com/user-attachments/assets/7dbe6c0f-bb04-4322-b914-e84954d8d29f" />


## Multiplication alp 
```
Org 100h
Mov ax, [1100h]
Mov bx, [1102h]
Mul bx
Mov [1200h], ax
Mov [1202h], dx
ret
```
 ## Output  
<img width="1625" height="935" alt="Screenshot 2026-11-18 000836" src="https://github.com/user-attachments/assets/38822a47-e8d7-4b0f-8ded-ba84f7a8f9a6" />


## Division alp 
```
Org 100h
Mov ax, [1100h]
Mov bx, [1102h]
Mul bx
Mov [1200h], ax
Mov [1202h], dx
ret
```

## Output  
<img width="1656" height="987" alt="Screenshot 2026-11-18 001053" src="https://github.com/user-attachments/assets/0c46d2ed-cca6-4ce2-a77e-f96a117bd315" />


## Logical AND alp
```
Org 100h
Mov bx, [1100h]
Mov cx, [1102h]
And bx,cx
ret
```
##  Output
<img width="1546" height="1020" alt="Screenshot 2026-11-18 082257" src="https://github.com/user-attachments/assets/47442e30-720f-4693-930d-893429cb9027" />

## Logical OR alp
```
Org 100h
Mov bx, [1100h]
Mov cx, [1102h]
OR bx,cx
ret
```
## Output
<img width="1480" height="985" alt="Screenshot 2026-11-18 082422" src="https://github.com/user-attachments/assets/ca50df0c-df88-4031-90d7-18e450289302" />

## Logical NAND alp
```
Org 100h
Mov bx, [1100h]
Mov cx, [1102h]
AND bx, cx
NOT bx
ret
```
## Output
<img width="1441" height="1012" alt="Screenshot 2026-11-18 082633" src="https://github.com/user-attachments/assets/8d069fbb-0efb-4520-bbfc-ead03fc229b4" />

## Logical NOR alp
```
Org 100h
Mov bx, [1100h]
Mov cx, [1102h]
OR bx,cx
NOT bx
ret
```

## Output
<img width="1490" height="1021" alt="Screenshot 2026-11-18 082741" src="https://github.com/user-attachments/assets/7950a039-005a-48b8-b34f-8d546613c806" />

## Logical XOR alp
```
Org 100h
Mov bx, [1100h]
Mov cx, [1102h]
XOR bx,cx
ret
```

## Output
<img width="1476" height="1025" alt="Screenshot 2026-11-18 082936" src="https://github.com/user-attachments/assets/5dccf30e-4e6a-403b-ba5d-2f2ef4d99d74" />

## Logical EX-NOR alp
```
Org 100h
Mov bx, [1100h]
Mov cx, [1102h]
XOR bx,cx
NOT bx
ret
```
## Output

<img width="1486" height="1026" alt="Screenshot 2026-11-18 083030" src="https://github.com/user-attachments/assets/af1c86fa-ae41-49f3-a5ed-f6c746fe90cf" />


## Result :
Thus the execution of ALP on fundamental arithmetic and logical operations was executed successfully 









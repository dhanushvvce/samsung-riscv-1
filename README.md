# samsung-riscv
## Basic Details

Name: CHETHAN V

College: Vidyavardhaka College of Engineering

Email ID: chethanvenugopal@gmail.com

GitHub Profile: chethankashyap24

LinkedIN Profile: chethanvenugopal

<details>
<summary> <b>Task 1:</b></summary>
<br>
The task involves referring to lab videos on C programming and RISC-V, and performing the compilation of C code using both the GCC compiler and the RISC-V compiler.
   
## C Language
### Compilation using GCC Compiler

Steps to compile any `.c` file :

1. Open the bash terminal and navigate to the directory where you want to create your file.
2. Run the following command to create and open the file in the editor:
   ```bash
   gedit sum1ton.c
3. Use these commands to run the C code:
    ```bash
   gcc sum1ton.c
   ./a.out
![sum1ton code](https://github.com/user-attachments/assets/1d88196a-812d-4977-bc33-75df96489417)

## RISC-V
Compile the code using the RISC-V GCC compiler using these commands:
1. Display c code:
   ```bash
   cat sum1ton.c
2. Command to compile code
   ```
   riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
3. Displays the assembly language code
   ```
   riscv64-unknown-elf-objdump -d sum1ton.o
![riscv1](https://github.com/user-attachments/assets/0aa98971-6197-417c-9e0a-6d9d5a561225)

4. Type `/main` to locate the main section in code
   
![RISCV2](https://github.com/user-attachments/assets/a844c11d-190c-4347-b937-49bc490f7166)

</details>

<details>
<summary><b>Task 2:</b></summary>
<br>
This task involves comparing two optimization levels, -O1 and -Ofast, while debugging a simple C program using SPIKE.

## Debugging with SPIKE

![VirtualBox_vdsworkshop_13_01_2025_19_06_42](https://github.com/user-attachments/assets/cbd9a387-1df4-40c2-aa91-e320ec984e4e)

The C code was compiled

In order to balance compilation time and performance, the -O1 optimisation option offers modest optimisation. It's perfect for a combination of performance enhancements that don't significantly affect debugging. Conversely, -Ofast aggressively optimises for optimal performance, even at the expense of adhering to some standard-compliant behaviours and possibly making debugging more difficult.
The code undergoing these optimisations can be seen in the attached file.

![VirtualBox_vdsworkshop_13_01_2025_20_52_37](https://github.com/user-attachments/assets/dd1b5a49-59ba-4201-b9de-1f3920afdd64)

Each optimisation level's RISC-V object dump (-O1 and -Ofast).

By disassembling the object file, the riscv64-unknown-elf-objdump tool reveals the machine code produced by each optimisation level:
The code undergoing these optimisations can be seen in the attached file.

![VirtualBox_vdsworkshop_13_01_2025_20_45_01](https://github.com/user-attachments/assets/0a9328fe-86de-4102-adf0-a6120fb4bfdf)

![VirtualBox_vdsworkshop_13_01_2025_20_44_40](https://github.com/user-attachments/assets/f4baee36-9df7-4291-91d4-aa6b0540f90a)

</details>





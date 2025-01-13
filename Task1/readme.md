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

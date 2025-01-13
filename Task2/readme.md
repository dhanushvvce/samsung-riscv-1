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

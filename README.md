# FreeRTOS_RISC-V QEMU
FreeRTOS on RISC-V QEMU for spike machine

1. Install riscv-gnu tools.
2. Install RISC-V QEMU
3. Go to FreeRTOS/Demo/riscv-spike and edit makefile.inc for gcc path setup 
4. Build FreeRTOS using make command on terminal and it generates riscv-spike.elf file
5. copy riscv-spike.elf file into RISC-V QEMU root folder and go to RISC-V QEMU root folder from command line.
6. run "./riscv64-softmmu/qemu-system-riscv64 -machine spike_v1.9 -kernel riscv-spike.elf -nographic"
   or   "./riscv64-softmmu/qemu-system-riscv64 -machine spike_v1.10 -kernel riscv-spike.elf -nographic" 

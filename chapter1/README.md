# Chapter 1 - Setting up a basic development environment

First of all, we choose to develop our kernel under Linux. This chapter is mainly to help readers set up a basic kernel development environment.

We divide the kernel development cycle into five steps:

1. Editing

   I use `emacs` locally. You can use another editor

2. Compiling and Assembly

   Here we need `GCC >= 4.7.1`. Of course we could use `clang`, but some compilation parameters of `clang` may be different.

   We are going to use `yasm` instead of `nasm` as an assembler. `yasm` is compatible with `nasm`, the difference is that `yasm` has more features. We can see later that `yasm` can modify the `ELF` attributes for functions written in assembly

3. Link

   Here we use `GNU ld`

4. Run

   For the running steps, we need to package the linked kernel first, generate an image file through the tool chain provided by `GRUB`, and put it in the virtual machine to run. Here we use `qemu-system-i386`. 

5. Debugging

   Only `GDB` is needed here, no other tools are needed. If you need a more powerful `gdb` front-end, you can go to `github` and search for `gdbgui`



In my environment (`ArchLinux`), the packages have been summarized below. 

1. `yasm`
2. `gcc`
3. `gdb`
4. `grub`
5. `mtools`
6. `xorriso`
7. `qemu-arch-extra` (as long as you have `qemu-system-i386`)
8. `git` (version management)

For `Ubuntu`/`Debian`/`Kali`, the packages are as follows.

1. `yasm`
2. `gcc`
3. `gdb`
4. `grub-common`
5. `grub-pc-bin`
6. `mtools`
7. `xorriso`
8. `qemu-system-x86`
9. `git`

Look in the `Makefile` to understand the dependencies.

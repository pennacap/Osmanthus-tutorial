# Chapter0 - Preface

This tutorial aims to help readers build a simple kernel through a step-by-step analysis.

Our target is:

1. Booting via GRUB
2. VGA mode compatible driver
3. Format printing function and kernel debugging function
4. Setting the GDT
5. Setting the IDT
6. Interrupt management
7. Timer programming
8. Physical Memory management
9. Virtual Memory Management
10. Kernel Heap Management
11. Kernel-level multithreading



Most of this tutorial refers to the [Implementation of the x86-based operating system kernel](http://wiki.0xffffff.org). Of course, there are some improvements and bugs, and the specific details are different. In any case , I admire the author Liu Huan for his ability to write such a high-quality blog.

Of course there is [JamesM's kernel development tutorials](http://www.jamesmolloy.co.uk/tutorial_html/). To be honest, I didn’t refer to it much. [OSDEV's Wiki](https://wiki.osdev.org/James_Molloy's_Tutorial_Known_Bugs) caught a bunch of bugs and weird problems.

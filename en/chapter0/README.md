# Chapter0 - Preface

This tutorial aims to help readers build a simple kernel through a step-by-step analysis.

Our target is:

1. Booting via GRUB
2. VGA compatible mode driver
3. Format printing function & kernel debugging function
4. Set up the GDT 
5. Set up the IDT
6. Interrupt management
7. Program the timer 
8. Physical memory management
9. Virtual Memory Management
10. Kernel Heap Management
11. Kernel-level multithreading

Most of this tutorial refers to [Implementation of the x86-based operating system kernel](http://wiki.0xffffff.org), of course there are some improvements and bugs, and the specific details are different. Anyway , I admire the author Liu Huan for writing such a high-quality blog.

Of course there is [JamesM's kernel development tutorials](http://www.jamesmolloy.co.uk/tutorial_html/). To be honest, I didn’t refer to it much, it looks pretty good, and I found out when I went deep into it, it’s too crude. [OSDEV's Wiki](https://wiki.osdev.org/James_Molloy's_Tutorial_Known_Bugs) caught a bunch of bugs and weird problems, but they still have some effect.

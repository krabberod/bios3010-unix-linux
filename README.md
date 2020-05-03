# Page for BIOS3010 - Introduction to UNIX

This part of the course will show you how to access and use the supercomputer Saga and how to use UNIX (and Linux) commands.

[Saga](https://www.sigma2.no/systems#saga) is a brand new high performance computing cluster put online in the fall of 2019. It's maintained by [Sigma2](https://www.sigma2.no/) and is one of several national supercomputers available for researchers. It has 200 standard compute nodes, with 40 cores and 192 GiB memory each, and in addition there are some specialized nodes (e.g. high-memory nodes with 3TiB memory or GPUs).

Saga like most [supercomputers](https://en.wikipedia.org/wiki/Supercomputer_operating_systems) runs some version of Linux. In order to access and do stuff on Saga you need to learn some basic Linux (and UNIX-style) commands.

### Linux vs. UNIX
Short version: UNIX has been called the mother of all operating systems (OS). The origin dates back to the mid 1960's when it was developed by people at MIT, Bell Labs and General Electrics to control some of their early computer frames. Linux is an open-source UNIX clone written by Linus Torvalds (first released in 1991), and the kernel of the MacOS is build on a UNIX-like framework. So when we use the term UNIX in this course it largely means the UNIX-style of running programs.  Common is the idea that the code should be simple, short, clear, modular, and extensible. It means that the programs
- should do one thing and do it well.
- work together.
- should handle text streams, because that is a universal interface.
If you want to dig deeper into the differences between UNIX/linux and MacOS you can for instance watch [Gary Explains UNIX vs Linux](https://youtu.be/jowCUo_UGts) on Youtube.


### Software
In order to get started you will need a shell. An we will cover that topic in Exercises 1.

**Mac and Linux** machines already have a [terminal](https://en.wikipedia.org/wiki/Terminal_emulator) with access to UNIX/linux style commands. You don't have to do any extra installation of programs for accessing saga, but if you want to be a pro you call always [pimp your bash](https://www.itworld.com/article/2833199/3-ways-to-pimp-your-bash-console.html).

**Windows**
To get a terminal with a functionality resembling that of a Linux machine on Windows you will have to install Git for Windows, or something similar (Cygwin, Console, ConEmu). This will be explained in Exercise 1.

### Exercises
1) [Logging on to Saga](Exercises/Exercise_1.md)
2) [Directory structures](Exercises/Exercise_2_folder_structure.md)
3) [Common commands](Exercises/Exercise_3_cmds.md)

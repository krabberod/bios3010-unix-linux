# Page for BIOS3010-unix

This part of the course will show you how to access and use the supercomputer Saga and how to use UNIX (and linux) command.

[Saga](https://www.sigma2.no/systems#saga) is a brand new cluster of CPUs that were put online in the fall of 2019. It's maintained by [Sigma2](https://www.sigma2.no/) and is one of several national supercomputers available for research. It has 200 standard compute nodes, with 40 cores and 192 GiB memory each, and in addition there are some specialised nodes (e.g. high-memory nodes with 3TiB memory or GPUs).

Saga like most [supercomputers runs some version of linux](https://en.wikipedia.org/wiki/Supercomputer_operating_systems). In order to access and do stuff on Saga you need to learn some basic linux (and unix-style) commands.

### Linux vs. Unix
Short version: UNIX has been called the mother of all operating systems (OS). The origin dates back to the mid 1960's when it was developed by people at MIT, Bell Labs and General Electrics to control some of their early computer frames. Linux is an open-source UNIX clone written by Linus Torvalds (first released in 1991), and teh kernel of the MacOS is build on a unix-like framework. So when we use unix in this course it largely means the unix-style of running programs.  Common is the idea that the code should be simple, short, clear, modular, and extensible. It means that the programs
- should do one thing and do it well.
- work together.
- should handle text streams, because that is a universal interface.
If you want to dig deeper into the differences between unix/linux and MacOS you can for instance watch [Gary Explains Unix vs Linux](https://youtu.be/jowCUo_UGts) on Youtube.



##Software:
In order to get started you will need a shell

### Mac and Linux
Since Mac and Linux users already have a terminal with access to unix/linux style commands you don't have to do any extra installation of programs for accessing saga.

### Windows
To get a terminal with a functionality resembling that of a Linux machine on Windows you will have to install [Git for Windows](https://gitforwindows.org/), or something similar (Cygwin, Console, ConEmu).

### Exercises
1) Logging on to Saga
2) Folder structure

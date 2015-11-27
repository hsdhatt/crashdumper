# crashdumper
linux kernel space crash dumper - Analyse the kernel space for potential bugs.

Design:

Create a loadable linux kernel module - crashdumper.ko
Upon a crash or kernel panic, this module will collect the entire ram data and send it to the server.
The transfer protocol to be used can be either over ethernet, or USB, or Serial.


Things to dump:
1. RAM dump
2. Linux kernel timers
3. page structs?
4. list of processes
5. locks - mutexes and spinlocks

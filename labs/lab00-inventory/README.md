# Lab 0 — Inventory your own machine

Pair: DAMIR NIYAZBEK (My pair) <br/>
Driver first half: TAMERLAN SHAKENOV (Me) <br/>
Machine: HP Victus 16-e0XXX (Laptop) <br/>
Date: 08.10.2026

## What I did
I used Windows PowerShell to collect information about my personal laptop, including the operating system, hardware specifications, processor, memory, and storage. Here are the commands I used:
Overview - Get-ComputerInfo <br/>
Memory - systeminfo <br/>
Disks - Get-Volume <br/>
OS - systeminfo <br/>
Virtualisation - systeminfo (on the bottom of the output) Hyper-V Requirements

```
Get-ComputerInfo
![image alt](https://github.com/Tashyouu/OSA/blob/main/labs/lab00-inventory/evidence/OS.png) <br/>
systeminfo
![image alt](https://github.com/Tashyouu/OSA/blob/2cfda98aeb53a8aa178b651e065b84a25c0769f4/labs/lab00-inventory/evidence/OS%20CPU%20MEMORY.png) <br/>
![image alt](https://github.com/Tashyouu/OSA/blob/2cfda98aeb53a8aa178b651e065b84a25c0769f4/labs/lab00-inventory/evidence/HYPER-V.png) <br/>
Get-Volume
![image alt](https://github.com/Tashyouu/OSA/blob/2cfda98aeb53a8aa178b651e065b84a25c0769f4/labs/lab00-inventory/evidence/DISKS.png) <br/>
```

## Result
Successfully collected basic system information using Windows PowerShell. The inventory included the operating system, processor, installed memory, storage devices, and computer model.

The commands demonstrated how to query Windows system information using built-in PowerShell commands without installing additional software.

## What did not work the first time
During the inventory, some command output was not immediately obvious to interpret. For example, the installed memory (RAM) was displayed in megabytes rather than gigabytes.
I identified the value as the total physical memory and understood that it needed to be converted into gigabytes for easier reading.

## Evidence

- [evidence/](https://github.com/Tashyouu/OSA/blob/2cfda98aeb53a8aa178b651e065b84a25c0769f4/labs/lab00-inventory/evidence/DISKS.png) — Disks info. [evidence/] (HYPER-V.png/)
- [evidence/](HYPER-V.png/) — Hyper-V (Virtualisation) info.
- [evidence/](OS_CPU_MEMORY.png/) — OS, CPU and RAM memory info.
- [evidence/](OS.png/) — OS info that is shown by using 'overview' command.

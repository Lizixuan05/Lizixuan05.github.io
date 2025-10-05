---
title: "龙芯杯项目作品"
excerpt: "High-Performance Superscalar Processor and Its System-on-Chip (SoC)<br/><img src='/images/architecture.png'>"
collection: portfolio
---

This project is the entry of the **Cache Miss Reboot (CMR)** team in the 9th “Loongson Cup” competition. In this project, we successfully developed a CPU based on the **LA32R instruction set**, named **CMR (Cache Miss Reboot)**. The CMR processor is built upon the **Tomasulo bypass algorithm**, featuring an **11–13 stage pipeline**, **multiple issue**, **out-of-order execution**, and **in-order commit**. It supports **precise exception handling**, **virtual address translation**, and handling of various interrupts and exceptions.

The CMR processor can **stably run functional and performance tests**, achieving a **maximum clock frequency of 95 MHz**. With **pre-decoding techniques** and **cache optimizations**, CMR achieves an overall **speedup of 4.183** and an **IPC speedup of 1.438** compared to the baseline **openLA500 processor (33 MHz)**. Furthermore, CMR can **reliably boot the Linux operating system via the U-Boot bootloader** and execute corresponding applications.

We also designed the **CMR-SoC system**, which integrates all on-board peripheral interfaces and successfully drives all peripherals **except PS2 and USB**. Corresponding modifications were made to the system software to ensure compatibility, and **MicroPython was successfully ported**, allowing Python applications to run on our development board. 

Additionally, combined with our **self-developed one-click toolchain**, we implemented **fully automated and efficient workflows** from microarchitecture design and functional development to on-board testing. Guided by **quantitative research methods**, we rigorously explored the **optimal performance of parameterized configurations** through systematic experimentation.

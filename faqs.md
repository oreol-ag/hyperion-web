# FAQs

## What type of accelerator is a multi-core CPU? 
A multi-core CPU (Central Processing Unit) is a **scalar processor** that contains multiple processing cores on a single chip, each of which can execute instructions independently of others. While multi-core CPUs are not typically considered accelerators like GPUs or FPGAs, they can provide a significant performance boost for certain types of workloads, particularly those that involve a mix of sequential and parallel computations for multi-threaded applications.

## What type of accelerator is a GPU? 
A GPU (Graphics Processing Unit) is a **vector processing device**  initially designed to accelerate graphical computations by performing many calculations in parallel on large sets of data, such as pixels in an image or vertices in a 3D model. In recent years, GPUs have been used for other applications beyond graphics, such as scientific computing, machine learning, or cryptography. All these use cases (as well as image processing tasks) require calculations that can be done more efficiently using vector-based techniques that allow for the simultaneous parallel processing of multiple data elements.

Modern GPUs typically have hundreds (or even thousands) of processing cores and specialized hardware for handling vector operations—such as SIMD (Single Instruction Multiple Data) units.

## What type of accelerator is an FPGA? 
An FPGA (Field Programmable Gate Array) is commonly classified as a **spatial processing device.** They benefit from a different computational model, coding styles, and forms of parallelism than traditional Instruction Set Architecture (ISA) processors, including CPUs and GPUs, which are more familiar to most people.

Unlike traditional ISA processors—designed to execute a sequence of memory-stored instructions in a program, running on a fixed hardware architecture that can run different instructions at different times—FPGAs start from the opposite perspective. Instead of being based around a machine that executes instructions on shared hardware, spatial implementations of a program conceptually take the entire program and lay it down at once on the device. This way, each instruction in the program receives its dedicated hardware that can execute simultaneously (in the same clock cycle) as all other instructions in the program—as they are spatially decoupled in the device. 

In many ways, this differs from sharing hardware between instructions over time, as it happens with scalar and vector processor devices.
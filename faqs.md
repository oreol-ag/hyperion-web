<div id="readme" class="Box-body readme blob js-code-block-container">
<article class="markdown-body entry-content p-3 p-md-6" itemprop="text">
<p align="right">
<a href="https://github.com/oreol-ag/hyperion#--heterogenius-computing">Back to top</a>
</p>

# FAQs

The following are frequently asked questions about **Hyperion and its hardware accelerators.**

## What is Hyperion?
Hyperion is a ready-to-use acceleration platform combining energy-efficient servers with advanced acceleration devices such as ACAPs, FPGAs, multi-core CPUs, and GPUs. It also includes a customized command-line interpreter (CLI) and an API, bundled as Hyperion RunTime (HRT), for seamless management and programming of these devices.

## Who is Hyperion intended for? 
Hyperion is created to simplify the process of developing complex acceleration applications, primarily serving highly specialized acceleration engineers working at research institutions or universities. These engineers typically benefit from dedicated on-site hardware for development, testing, and staging before transitioning to production.

## Is Hyperion hosted in the public cloud? 
No, Hyperion is designed to be an on-premises resource for edge computing. However, you have the option to build your private cloud using Hyperion servers and offer your accelerated services by exposing them.

## How can I begin using Hyperion? 
You can get started by trying out a few Hyperion instances available online for free evaluation. Simply sign in here to give it a try.

## How can I purchase Hyperion? 
To obtain Hyperion instances, please complete this form, and our sales department will reach out to you shortly.

## How are my Hyperion instances maintained? 
Hyperion is a managed platform, allowing us to provide remote maintenance for your Hyperion servers. We ensure the health and keep them up-to-date, including the operating system, acceleration development tools, and the devices themselves.

## How do I  build accelerated applications on Hyperion? 
Hyperion includes Hyperion RunTime (HRT), featuring a CLI and an API. The command-line interpreter assists in building customized accelerated applications—tailored to your Hyperion instance's underlying hardware—and sets up the infrastructure accordingly. Additionally, the API streamlines development, allowing seamless utilization of all exposed devices (ACAPs, FPGAs, multi-core CPUs, and GPUs) in your source code.

## What type of accelerator is a multi-core CPU? 
A multi-core CPU (Central Processing Unit) is a **scalar processor** that contains multiple processing cores on a single chip, each of which can execute instructions independently of others. While multi-core CPUs are not typically considered accelerators like GPUs or FPGAs, they can provide a significant performance boost for certain types of workloads, particularly those that involve a mix of sequential and parallel computations for multi-threaded applications.

## What type of accelerator is a GPU? 
A GPU (Graphics Processing Unit) is a **vector processing device**  initially designed to accelerate graphical computations by performing many calculations in parallel on large sets of data, such as pixels in an image or vertices in a 3D model. In recent years, GPUs have been used for other applications beyond graphics, such as scientific computing, machine learning, or cryptography. All these use cases (as well as image processing tasks) require calculations that can be done more efficiently using vector-based techniques that allow for the simultaneous parallel processing of multiple data elements.

Modern GPUs typically have hundreds (or even thousands) of processing cores and specialized hardware for handling vector operations—such as SIMD (Single Instruction Multiple Data) units.

## What type of accelerator is an FPGA? 
An FPGA (Field Programmable Gate Array) is commonly classified as a **spatial processing device.** They benefit from a different computational model, coding styles, and forms of parallelism than traditional [Instruction Set Architecture (ISA) processors,](./vocabulary.md#instruction-set-architecture-isa-processors) including CPUs and GPUs, which are more familiar to most people.

Unlike traditional ISA processors—designed to execute a sequence of memory-stored instructions in a program, running on a fixed hardware architecture that can run different instructions at different times—FPGAs start from the opposite perspective. Instead of being based around a machine that executes instructions on shared hardware, spatial implementations of a program conceptually take the entire program and lay it down at once on the device. This way, each instruction in the program receives its dedicated hardware that can execute simultaneously (in the same clock cycle) as all other instructions in the program—as they are spatially decoupled in the device. 

In many ways, this differs from ISA devices: an FPGA does not have a pre-defined instruction set, and the logic functions it performs are entirely determined by the user's programming; furthermore, they do not share hardware between instructions over time—as it happens with scalar and vector processors.

## What type of accelerator is an ACAP?
An ACAP (Adaptive Compute Acceleration Platform) is a type of programmable hardware accelerator that combines the capabilities of both GPUs (Graphics Processing Units) and FPGAs (Field Programmable Gate Arrays) into a single platform.

Like GPUs, ACAPs have a high number of processing cores and specialized hardware for handling vector-based operations and other compute-intensive tasks. Like FPGAs, ACAPs have a re-programmable spatial processing region that benefits from such architectures by performing application-specific operations in dedicated reconfigurable hardware.

Overall, ACAPs are designed to provide a flexible and adaptable platform for accelerating a broader type of compute-intensive workloads in a single device.

## Is my application GPU- or FPGA-like?
FPGAs (Field-Programmable Gate Arrays) and GPUs (Graphics Processing Units) are both powerful computing platforms, but they have different strengths and weaknesses that make them suitable for different types of applications. In general, GPUs are better for applications that require massive parallelism and high-throughput computation, while FPGAs are best suited for applications that require high-speed data processing and low-latency operation.

Some examples of applications that are better suited for GPUs include:

1. Graphics rendering and video game development
2. Scientific computing and simulations
3. Machine learning training
4. Cryptocurrency mining

On the other hand, some examples of applications that are better suited for FPGAs include:

1. Real-time signal processing and digital signal processing (DSP)
2. High-frequency trading (HFT) and financial modeling
3. Machine learning inference and deep learning
4. Network packet processing and network security
5. Video and image processing

However, with Hyperion both FPGAs and GPUs can be used in conjunction with each other to accelerate complex workloads that require both parallel processing and low latency.
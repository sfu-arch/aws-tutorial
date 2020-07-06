# AWS-Tutorial
This repo contains summary of [Amazon AWS repository](https://github.com/aws/aws-fpga) documentation about how to use F1 instances. We have reorganized the documentation, add more explanation in cases that we feel it is needed, **Troubleshooting** section for each part, and explain how to connect [muIR](https://github.com/sfu-arch/muir-sim) to the rest of the system.

## AWS User setup
In this tutorial we have provided details instructions about how to setup your AWS account for the first time and install prerequisites. If you have never used AWS before, this is the best starting point for you.

** [First-time AWS User Setup](./docs/setup_account.md) **

## HLS Tutorial
Our first tutorial starts by explaining how Xilinx HLS framework works on AWS machines. In this tutorial you will learn how to build your custom C + pragmas or OpenCL program on AWS and benchmark your application. In this tutorial you will learn:

1. The overall F1 FGPA -- Host architecture and memory addresses
2. How to simulate and validate your HLS design
3. How to compile and build FPGA binary
4. How to upload your binary to Amazon S3 buckets to make it available for F1 instances
5. Load your FPGA image to F1 instance and run your binary
6. Finally we explain possible errors that you may end up with

** [Guide to Accelerating your C/C++ application on an AWS F1 FPGA Instance with SDAccel](./docs/hls.md) **


## Custom Logic (CL) Hello World Example
In this tutorial, we explain amazon AWS hello world custom logic example. The "Hello World" example exercises the `OCL` Shell-to-CL AXI-Lite interface, the Virtual LED outputs and the Virtual DIP switch inputs. This page will walk through the custom logic RTL (Verilog), explain the AXI-lite slave logic, and highlight the PCIe APIs that can be used for accessing the registers behind the AXI-lite interface.

** [Custom Logic (CL) Hello world example](./docs/cl_hello_world.md) **

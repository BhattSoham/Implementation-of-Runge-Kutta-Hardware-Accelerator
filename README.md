# Hardware Acceleration in solving ODE using Runge Kutta methods #

Hardware acceleration is crucial in enhancing performance, efficiency, and scalability across a wide range of computing applications. In this work, we have implemented a hardware accelerator specifically used for a Runge-Kutta Solver for solving an ordinary differential equation. Runge Kutta numerical methods are widely used to solve ordinary differential equations (ODEs). Among the Runge Kutta methods, RK2, RK3, and RK4 are commonly used variants for approximating the solutions to the differential equations. The hardware accelerators have been implemented using the VHDL programming language and deployed on the Zynq ZC702 FPGA evaluation board. A comprehensive comparative analysis of different Runge-Kutta hardware accelerators, highlighting factors including timing performance, hardware resource usage, and the total on-chip power consumption has been given. According to the experimental findings, the fourth-order Runge-Kutta equation has a significant power consumption, rising by
an estimated 51.37 percent and 12.445 percent when comparing second-order and third-order Runge-Kutta solvers at a clock rate of 100 MHz, respectively. This
study contributes to the enhancement of ODE solutions in high-performance computing applications. This work has been published in the **IEEE ICECCE 2023** conference. [https://ieeexplore.ieee.org/document/10442325] 

The documentation for downloading Xilinx Vivado and the tutorial for using VHDL has been given below:

Xilinx Vivado: [https://docs.xilinx.com/r/2022.1-English/ug973-vivado-release-notes-install-license/Download-and-Installation]

VHDL Tutorial: [https://www.eecs.umich.edu/courses/doing_dsp/handout/vhdl-tutorial.pdf]

Let's Start!

For implementing the design using RK2, RK3, and RK4 methods, Xilinx Vivado's single precision floating point IP support has been used. The specifications are given below:

| ODE solvers                   |FPU_ADD        | FPU_SUB            |FPU_MUL                |MAC_units        |     
| ------------------------------| ------------- |-------------       |------------           |-----------------|
| RK2                           | 6             |1                   |4                      |X                |
| RK3                           | 5             |2                   |5                      |4                |   
| RK4                           | 7             |1                   |2                      |4                |

All the other details for implementation have been given in the specific directories.




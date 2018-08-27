---
layout: page
title: "Program"
teaser: ""
header:
   image_fullwidth: "belfast.jpg"
   permalink: "/program/"
---

<h3>Schedule</h3>

**09h00**: Welcome

**09h15**: Keynote: Resilience For Extreme Scale Systems: From Root Causes to Solutions (Christian Engelmann, Oak Ridge National Laboratory, USA)

**10h30**: Coffee Break

**11h00**: A Failure Prediction-based Adaptive Checkpointing Method with Less Reliance on Temperature Monitoring for HPC Applications (Muhammad Alfian Amrizal, Pei Li, Mulya Agung, Ryusuke Egawa and Hiroyuki Takizawa)

**11h35**: Challenges in Developing MPI Fault-Tolerant Fortran Applications (Nathan Weeks, Glenn Luecke, Pieter Maris and James Vary)

**12h10**: Closing

**12h15**: End

<h3>Keynote details</h3>
Resilience is one of the critical challenges of extreme-scale high-performance computing (HPC) systems. 
This talk provides an overview of two different projects addressing these issues, the Catalog project and the 
Resilience Design Pattern project. The Catalog project develops a fault taxonomy, catalog and models that capture 
the observed and inferred conditions in current supercomputers and extrapolates this knowledge to future-generation 
systems. To date, this project has analyzed billions of node hours of system logs from supercomputers at Oak Ridge 
National Laboratory and Argonne National Laboratory. The Resilience Design Pattern project offers a structured 
approach to the design, evaluation and optimization of HPC resilience using the concept of design patterns. 
It identifies the problems caused by faults, errors and failures in HPC systems and the techniques used to deal with 
these events.

<h3>Paper details</h3>

**A Failure Prediction-based Adaptive Checkpointing Method with Less Reliance on Temperature Monitoring for HPC Applications**

Checkpointing with a constant checkpoint interval is optimal assuming an exponential distribution of failures. However, in practice there are many events that correlate with failures, such as CPU temperature. Under these circumstances, adaptive checkpoint intervals are more appropiate, but require extra overhead to monitor the system. In this paper, we propose an adaptive checkpointing method that avoids constant monitoring by using timings of the already occurred failures, called the prior failures, to estimate the mean time to failure (MTTF) of the next failure, called the posterior failure. The simulation results show that the proposed method can reduce the total wasted time compared to the constant checkpointing method with a considerably small temperature monitoring period.

**Challenges in Developing MPI Fault-Tolerant Fortran Applications**

Powerful high performance computing systems of the future are expected to have higher failure rates than current systems. The MPI 3.1 standard does not address the issue of MPI process failures. Checkpoint/restart is commonly used to add fault tolerance to MPI applications, however this can have a high overhead. Several MPI fault tolerance libraries, such as ULFM, are being developed to enable MPI programs to recover from MPI process failures. This can circumvent much of the overhead of an application restart, including rescheduling, launching, initializing, and reading checkpoint data. Each library uses a different approach to recovery from MPI process failures. Unfortunately, some of the proposed recovery models are incompatible with Fortran. This paper intends to help Fortran MPI application developers avoid problems when developing fault-tolerant MPI applications.

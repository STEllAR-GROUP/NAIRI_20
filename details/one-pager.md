<!-- 
Copyright (c) 2020 R. Tohid (@rtohid)

Distributed under the Boost Software License, Version 1.0.(See accompanying
file LICENSE_1_0.txt or copy at http://www.boost.org/LICENSE_1_0.txt) 
-->

# Draft
Transcompiling high-level programs (e.g., Python) down to fast machine code
has been the subject of many studies [...] and resulted in immense success
specially on parallel machines (CPUs and GPUs). This has been a great
advantage for the AI community particularly with the rise of DNN where there
is abundance of parallelism in both algorithms and data. However, scaling
beyond one node, where cost of accessing data is significantly more, has been
a challenge, both in terms of finding elegant algorithms to deal with these
environments, and also software tools facilitating data movement between
nodes, i.e., through the network. Most efforts to overcome this challenge
have relied on fork-and-join paradigm, and commonly implemented close to
transformation layer on top of MPI. The fork-and-join model is inherently
vulnerable to idle time imposed by the synchronization step. In addition, 
although MPI is extremely efficient and portable, writing high-throughput on
top of it requires expert knowledge and Many works before This is one of ca
the reason behind the rise of DSLs in past decade. The greatest example would
be TensorFlow with all the tools the community built around it. This approach
has been very successful on a single machine, specially if abundant
parallelism is available.

Build on tripod of existing robust software:
1. HPX C++ standard conforming (10+ years and running) runtime, also:
   + widely used in opensource community and national labs:
     * Octo-Tiger
     * DCA++

   + supports dataflow programming paradigms; both CPU and GPU tasks.
     * control over **parallelism** and **concurrency** (<u>concurrency
       between nodes</u>)

   + backend of many existing libraries:
     * Phylanx
     * blaze, blaze_cuda
     * FleCSI
     * Kokkos

2. Python

3. [MLIR](https://mlir.llvm.org/docs/LangRef/) is designed to be used in three
different forms: 
   - a human-readable textual form **suitable for debugging**
   - an in-memory form **suitable for programmatic transformations and analysis**
   - a compact serialized form **suitable for storage and transport**

HPX is the only C++ standard conforming runtime:

   + widely used in opensource community and national labs.
   + supports dataflow programming paradigms.
   + backend of many libraries:
      * Kokkos
      * blaze
      * FleCSI

   1. HPX
   2. PhySL
   3. Visualization and HMI
   4. Configurable DSLs built on top

# References
- demystifying
- mlir
- tiramisu
- TensorFlow

<!-- 
Copyright (c) 2020 R. Tohid (@rtohid)

Distributed under the Boost Software License, Version 1.0.(See accompanying
file LICENSE_1_0.txt or copy at http://www.boost.org/LICENSE_1_0.txt) 
-->

# [NAIRI](https://www.nsf.gov/pubs/2020/nsf20604/nsf20604.htm)

---

# PhySL: Portable HPX Runtime for Python/AI Applications

## [The Heilmeier Catechism](https://www.darpa.mil/work-with-us/heilmeier-catechism):

> What are you trying to do?
>> Develop a runtime environment for AI applications. The goal is to build a
>> wholistic environment for development, testing, profiling, analysis and
>> deployment of AI programs. The system itself is also built with AI in mind
>> providing hooks and interfaces for extracting features and applying AI guided
>> dynamic policies. 
>>
>> In other words a transcompiler and the associated tools for AI development
>> and evaluation of applications running on anything between a RaspberryPi to
>> the Fujitsu ARM supercomputer.

> How is it done today, and what are the limits of current practice?
>> today:
>> - DSL languages (e.g. TensorFlow)
>> - optimization frameworks (e.g., Numba, Polly/Pluto, Tiramisu)
>> - many either built on top of or benefiting from LLVM IR.
>> - They have been immensely successful on a single node where there is
>>   abundance of parallelism and cost of accessing data is relatively low.
>> - distributed efforts mostly based on fork-join model and built on MPI
>> - MLIR is actively developed to alleviate some of the following limitations 
>>
>> limits:
>> - inherently vulnerable to synchronization steps leaving many computing
>>   resources idle.
>> - developing performant applications on top of MPI requires expert knowledge
>>   and therefore often not productive.
>> - one usually ends up using multiple programming languages to benefit from
>>   parallelism, for example through OMP and vectorization intrinsics which in
>>   turn are only available in lower level languages such as C++ and Fortran.
>> - the last point also means profiling and debugging application is not easily
>>   feasible.
>> - requires external libraries for data analytics on results as well as
>>   profiling of the system itself.

> What is new in your approach and why do you think it will be successful?
>> 1. Relying on second order derivatives 
>> 2. PhySL continues to use fork-join model when proven beneficial- for example
>>    on many core resources such as GPUs. However, it also improves concurrency
>>    and therefore throughput by relying on other programming constructs such
>>    as _data-flow_ and _futures_.
>> 3. It is built on top of the well established technologies such as HPX, 
>>    MLIR (successor of LLVM IR), Blaze, ... 
>> 4. HPX abstracts away many MPI programming's complexities, and PhySL makes it
>>    easy to build specializations on top of HPX.
>> 5. Uniform API for any programming paradigms, HPX light-weight threads
>>    running any tasks on CPUs and GPUs
>> 6. Easy profiling with integration of APEX
>> 7. Easy analysis with visualization of the profiling and trace data through
>>    Traveler.
>> 8. Phylanx have shown:
>>    - better or comparable performance on single node
>>    - better performance for distributed algorithm
>>    - JetLag facilitates application deployment (local and remote), also
>>      collects and visualizes profiling data.
>>    - easy to hook with third-party libraries such as Tiramisu
>>    - multi-granular performance analysis (PhySL task, HPX thread, ...)
>> 9. Already have the infrastructure for development and test (Rostam)

> Who cares? If you are successful, what difference will it make?
>> 1. Most of scientific community as they widely benefit from AI.
>> 2. Tightly related with the AI building blocks and can provide insights for
>>    better understanding of machine learning.
>> 3. Opensource community
>>    - liberal license
>>    - contribution to other opensource projects such as: LLVM, Python, Blaze, ...
>> 4. it would be nice if we can come up with concrete applications such as NLP
>>    or bioinformatics

> What are the risks?
>> It overarches many fields of study and requires many complex software work in
>> tune.
>> Time sensitive, it is crucial to plan and achieve well-defined goals.

> How much will it cost?
>> ??

> How long will it take?
>> 4-5 years?

> What are the mid-term and final “exams” to check for success?
>> mid-term (single machine):
>> - expand GPU
>> - enable triggering optimization through high-level directives (e.g., 
>>   decorators)
>> - prototype of new algorithms benefiting from concurrency in distributed
>>   systems.
>> - User guided deployment and profiling of application.
>>  
>>
>> long-term:
>> - capability to automatically detect and apply optimization based on the
>>   features of the program, e.g., affine, sparse, ...
>> - capability to automatically detect and apply optimization based on the
>>   system capacity, e.g., available memory, CPU, GPU, distributed ...
>> - interactive and intuitive user interface
>>    + Jupyter
>>    + Traveler integrated
>>    + Graph based visualization and analysis of control-flow graphs and
>>      execution-trees.
>> - develop efficient math and solver libraries on HPX.

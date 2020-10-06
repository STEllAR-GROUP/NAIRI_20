<!-- 
Copyright (c) 2020 R. Tohid (@rtohid)

Distributed under the Boost Software License, Version 1.0.(See accompanying
file LICENSE_1_0.txt or copy at http://www.boost.org/LICENSE_1_0.txt) 
-->

# Related Work

1. Second Order: 
   [1](http://proceedings.mlr.press/v28/sutskever13.pdf),
   [2](https://openaccess.thecvf.com/content_CVPR_2019/papers/Osawa_Large-Scale_Distributed_Second-Order_Optimization_Using_Kronecker-Factored_Approximate_Curvature_for_Deep_CVPR_2019_paper.pdf),
   [3](https://www.researchgate.net/profile/Roberto_Battiti/publication/2498372_First-_and_Second-Order_Methods_for_Learning_Between_Steepest_Descent_and_Newton%27s_Method/links/5537b11c0cf2058efdeae0b6/First-and-Second-Order-Methods-for-Learning-Between-Steepest-Descent-and-Newtons-Method.pdf)

2. Technologies
   - MLIR
      + [Language Reference](https://mlir.llvm.org/docs/LangRef/)
      + [Python binding](https://mlir.llvm.org/docs/Bindings/Python/)

   - [kokkos](https://github.com/kokkos/kokkos)
   - [HPX](https://github.com/stellar-group/hpx)
   - [SHAD](https://github.com/pnnl/SHAD)
   - [I/O](http://stellar.cct.lsu.edu/files/phylanx_kickoff/year_two_kickoff/kheirkhahan_io_operations_04.19.18.pdf)?


3. Libraries
   - [Phylanx](https://github.com/STEllAR-GROUP/phylanx/)
   - APEX
       + [src](https://github.com/khuck/xpress-apex)
       + [Performance Analysis](https://github.com/khuck/SC15_APEX_tutorial/blob/master/HPX_APEX_TAU_Tutorial_Slides.pdf)

   - Traveler
       + [src](https://github.com/hdc-arizona/traveler-integrated)
       + [Visualization](http://stellar.cct.lsu.edu/files/phylanx_kickoff/year_three-kickoff/presentations/isaacs_traveler.pdf)

   - JetLag
       + [src](https://github.com/STEllAR-GROUP/JetLag/pull/6)
       + [workflow](https://docs.google.com/presentation/d/1KhPByW69XtpKhAmcBvT3Ay1lvrFbYvG4XkJaV4rtcyg/edit#slide=id.p)

   - Blaze
       + [src](https://bitbucket.org/blaze-lib/blaze/src/master/), [GPU](https://github.com/STEllAR-GROUP/blaze_cuda/)
       + blazemark: [src](https://bitbucket.org/blaze-lib/blaze/src/master/blazemark/), [analyis](https://github.com/scheherzade/Blazemark/tree/master/data)
       + [HPX backend](http://stellar.cct.lsu.edu/files/phylanx_kickoff/year_three-kickoff/presentations/shirzad_blaze.pdf)

   - Tiramisu
      + Publications: 
        [1](https://arxiv.org/pdf/1804.10694.pdf),
        [2](https://arxiv.org/pdf/2005.04091.pdf)
      + [project](https://github.com/Tiramisu-Compiler/), [src](https://github.com/Tiramisu-Compiler/tiramisu/) repos

4. Past Slides
   [SC18](https://docs.google.com/presentation/d/1iN5_54EMknjB3JYY1m8cb4hYzV7gXWxBdJq8TO1lPyE/edit#slide=id.g4547084e32_0_0), 
   [JIT](https://docs.google.com/presentation/d/1kgI4TEXTRCLC7sfI6sht64WtlO-X_kLaoJ6VTB5YsNA/edit#slide=id.g28ef27b4a8_0_179), 
   [Blaze](https://docs.google.com/presentation/d/1Iaega8TctQX_EgcfnMk76evZD1AryhNrMTpe1Mxx8gg/edit#slide=id.g28ef27b4a8_0_179)
   
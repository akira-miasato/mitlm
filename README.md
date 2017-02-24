### DISCLAIMER: This is **not** the official GitHub repository for the MITLM utility
This is only a fork using the CMake build management utility
Check the official repository at https://github.com/mitlm/mitlm
Acknowledgements are reproduced from the official README at the end of the file

This project was created as an alternative to the autotools-based build management from the official repository. The CMakeLists.txt file is very minimal, so any contribution is welcome.

TODOs:
* Tests
* Portability assessment (specially with Fortran/C bindings)

Current tested environments:
* Ubuntu 14.04 with GCC/G++ 4.9.4 and equivalent libfortran/gfortran
* Ubuntu 16.04 with GCC/G++ 5.4.0 under ppc64le architecture

Dependency list (expected to work, file an issue if this is not the case):
* ANSI C++/Fortran compiler (GCC 4.7.1+)
* libgfortran (version should match your GCC's)
* CMake 2.8.12+

```
================
Acknowledgements
================

The design and implementation of this toolkit benefited significantly
from the SRI Language Modeling Toolkit by Andreas Stolcke.

The vector library is partially derived from the Flexible Library for
Efficient Numerical Solutions by Michael Lehn.

  Copyright (c) 2007, Michael Lehn

  All rights reserved.

  Redistribution and use in source and binary forms, with or without
  modification, are permitted provided that the following conditions
  are met:

  1) Redistributions of source code must retain the above copyright
     notice, this list of conditions and the following disclaimer.
  2) Redistributions in binary form must reproduce the above copyright
     notice, this list of conditions and the following disclaimer in
     the documentation and/or other materials provided with the
     distribution.
  3) Neither the name of the FLENS development group nor the names of
     its contributors may be used to endorse or promote products
     derived from this software without specific prior written
     permission.

  THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
  "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
  LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
  FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
  COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
  INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
  BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
  LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
  ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
  POSSIBILITY OF SUCH DAMAGE.

The project is supported in part by the T-Party Project, a joint
research program between MIT CSAIL and Quanta Computer Inc.

Bo-June (Paul) Hsu
Computer Science and Artificial Intelligence Laboratory
Massachusetts Institute of Technology
(C) 2008 
```



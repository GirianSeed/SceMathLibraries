# sceCellMath

This repository archives [Bullet](https://pybullet.org/wordpress/)'s revision history for the SIMD and vector math libraries for Cell/B.E. and x86 SSE contributed by [Sony Computer Entertainment Inc.](https://www.sie.com/index.html)

## Commit History

The history of the following directories has been transplanted to this repository.

* [Extras/simdmathlibrary](https://github.com/bulletphysics/bullet3/commits/47cae15fe5730c6a7ff8c3f745001d6ecd5106b2/Extras/simdmathlibrary) (as of commit [2579](https://github.com/bulletphysics/bullet3/commits/47cae15fe5730c6a7ff8c3f745001d6ecd5106b2/))

* [Extras/vectormathlibrary](https://github.com/bulletphysics/bullet3/commits/47cae15fe5730c6a7ff8c3f745001d6ecd5106b2/Extras/vectormathlibrary) (as of commit [2579](https://github.com/bulletphysics/bullet3/commits/47cae15fe5730c6a7ff8c3f745001d6ecd5106b2/))

Both directories were deleted in commit [2580](https://github.com/bulletphysics/bullet3/commit/2dfde77bacded1a1fca84dba63e58f4cdc47d97c).

Author        | Date         | Commit | Message
------------- | ------------ | ------ | -------
ejcoumans     | Jul 23, 2007 | 678    | Added SCE SIMD math library in Extras/simdmathlibrary [...]
ejcoumans     | Jul 23, 2007 | 679    | added missing file
ejcoumans     | Jul 23, 2007 | 680    | Added vectormath library, the open source version. Currently, PowerPC PPU, Cell SPU and a scalar version is available. [...]
ejcoumans     | Jul 24, 2007 | 681    | added SSE version of vectormath
ejcoumans     | Jul 25, 2007 | 682    | replaced alignment to use __declspec(align(16)) class VecIdx, instead of aligning the members __m128 &ref __attribute__ ((aligned(16)));
ejcoumans     | Jul 25, 2007 | 683    | added very quick/basic testfile+Makefile for vectormath under PS3 Linux 
ejcoumans     | Jul 25, 2007 | 684    | add stdc++ to linker
ejcoumans     | Jul 27, 2007 | 688    | added updated version of simdmathlibrary-1.0.1
ejcoumans     | Jul 27, 2007 | 689    | update vectormath to be 32bit PPU architecture
ejcoumans     | Jul 27, 2007 | 690    | added LICENSE and README
ejcoumans     | Jul 27, 2007 | 691    | added LICENSE and README
ejcoumans     | Aug 9, 2007  | 714    | removed comments from LICENSE file 
ejcoumans     | Aug 9, 2007  | 715    | removed C++ style comments from license file
ejcoumans     | Aug 10, 2007 | 716    | updated README with more details
ejcoumans     | Aug 10, 2007 | 717    | updated README with more details
ejcoumans     | Aug 15, 2007 | 726    | added tests for Vector Math, modified Makefile, added helper include files
ejcoumans     | Aug 15, 2007 | 727    | removed obsolete files
ejcoumans     | Aug 15, 2007 | 730    | Sony approved and provided an update to vec_types.h to use the BSD license.
ejcoumans     | Aug 16, 2007 | 731    | applied patch to improve build system
ejcoumans     | Aug 16, 2007 | 732    | patched makefile for tests, thanks to Kazunori Asayama 
ejcoumans     | Aug 16, 2007 | 733    | accidently overwrite the most recent version of README by an older one.
ejcoumans     | Aug 20, 2007 | 741    | forgot to add Make.* files
ejcoumans     | Aug 20, 2007 | 742    | patch to allow building of SPU version
ejcoumans     | Aug 21, 2007 | 743    | converted files to UNIX EOL
ejcoumans     | Feb 28, 2008 | 1056   | use newton-rapson iteration for more precise normalize() method
erwin.coumans | Nov 10, 2008 | 1497   | removed bloated reference docs, will add them in a separate package
erwin.coumans | Mar 6, 2010  | 2053   | fix: some file didn't have the svn:eol-style native yet
erwin.coumans | Apr 20, 2010 | 2088   | SCE Vectormath scalar version update
erwin.coumans | May 6, 2010  | 2091   | Minor update SSE version of SCE Vectormath library [...]

### Other Directories

* [src/BulletMultiThreaded/vectormath](https://github.com/bulletphysics/bullet3/commits/4eddfce03e947ea3610e40db27cffe3fb1709b1f/src/BulletMultiThreaded/vectormath) (as of commit [2132](https://github.com/bulletphysics/bullet3/commit/4eddfce03e947ea3610e40db27cffe3fb1709b1f))

  * moved to ``src/vectormath`` in commit [2133](https://github.com/bulletphysics/bullet3/commit/dd0f022d1daf65c7accc91369042f509a922a201)

* [src/vectormath](https://github.com/bulletphysics/bullet3/commits/976cd0028af569f384965af24b8196d948dade5f/src/vectormath) (as of commit [2636](https://github.com/bulletphysics/bullet3/commit/976cd0028af569f384965af24b8196d948dade5f))

  * deleted in commit [2637](https://github.com/bulletphysics/bullet3/commit/08272c7de5240f204532d282a92cfb76926d68ad)

* [test/Bullet2/vectormath](https://github.com/bulletphysics/bullet3/commits/master/test/Bullet2/vectormath)

## License

### SIMD Math Library

```
  SIMD math library functions for both the PowerPC (PPU) and the SPU.
   Copyright (C) 2006, 2007 Sony Computer Entertainment Inc. 
   All rights reserved.

   Redistribution and use in source and binary forms,
   with or without modification, are permitted provided that the
   following conditions are met:
    * Redistributions of source code must retain the above copyright
      notice, this list of conditions and the following disclaimer.
    * Redistributions in binary form must reproduce the above copyright
      notice, this list of conditions and the following disclaimer in the
      documentation and/or other materials provided with the distribution.
    * Neither the name of the Sony Computer Entertainment Inc nor the names
      of its contributors may be used to endorse or promote products derived
      from this software without specific prior written permission.

   THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" 
   AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
   IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
   ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
   LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
   CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
   SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
   INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
   CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
   ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
   POSSIBILITY OF SUCH DAMAGE.

```

### Vector Math Library

```
 Vector Math library for 3-D linear algebra (vector, matrix, quaternion)
   SIMD support for SSE, PowerPC (PPU) and the SPU.
   Also includes generic multi-platform scalar version. 

   Copyright (C) 2006, 2007 Sony Computer Entertainment Inc. 
   All rights reserved.

   Redistribution and use in source and binary forms,
   with or without modification, are permitted provided that the
   following conditions are met:
    * Redistributions of source code must retain the above copyright
      notice, this list of conditions and the following disclaimer.
    * Redistributions in binary form must reproduce the above copyright
      notice, this list of conditions and the following disclaimer in the
      documentation and/or other materials provided with the distribution.
    * Neither the name of the Sony Computer Entertainment Inc nor the names
      of its contributors may be used to endorse or promote products derived
      from this software without specific prior written permission.

   THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" 
   AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
   IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
   ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
   LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
   CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
   SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
   INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
   CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
   ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
   POSSIBILITY OF SUCH DAMAGE.

```

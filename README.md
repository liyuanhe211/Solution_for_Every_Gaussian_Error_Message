# Solutions for Gaussian Error Messages (migration work in progress)
This is an article containing reliable explanations and ways to solve the error messages for almost all common Gaussian quantum chemistry program. This is a per request English translation for [a long blog in Chinese](http://bbs.keinsci.com/thread-4829-1-1.html) I wrote a few years back. I wrote the original Chinese post as there are almost no reliable list of how to solve the errors. Similar online resources online are neither comprehensive nor accurate.

This blog is for people with basic knowledge of how Gaussian works, what's the basic structure of Gaussian files, and a basic understanding of quantum chemistry.

Using (part of) this blog in commercial setting (or for any profitable action) is prohibited. Otherwise feel free to use this material as long as you mention the source.

## List of errors
### General errors
 * [Severe Error Message # 2070 (Windows)](#SevereErrorMessage2070)
 * [segmentation violation/segmentation fault (Linux)](#SevereErrorMessage2070)
### QM related errors
 * [L1，ntrex1]
 * [L1，Illegal IType or MSType generated by parse.]
 * [L1，QPErr --- A syntax error was detected in the input line.]
 * [L101，End of file in ZSymb.]
 * [L101，WANTED A XXX AS INPUT. FOUND AN XXX AS INPUT.]
 * [L101，Input Error Input Error Input Error Input Error Input Error Input Error]
 * [L103，Error in internal coordinate system]
 * [L103，Linear angle in Bend; Linear angle in Tors]
 * [L103，FormBX had a problem]
 * [L103，NRF ne Abs NRFX]
 * [L103，New curvilinear step not converged. Error imposing constraints.]
 * [L114，ERROR IN INITNF. NUMBER OF VARIABLES (  0) INCORRECT (SHOULD BE BETWEEN 1 AND 50)]
 * [L202，Problem with the distance matrix.]
 * [L202，Atoms too close.]
 * [L123，Max corrector steps exceded]
 * [L123，GS2 Optimization Failure.]
 * [L123，GetHes: LRWHes > LHess!]
 * [L202，Atoms too close.]
 * [L301，The combination of multiplicity X and XXX electrons is impossible.]
 * [L301，End of file reading basis center.]
 * [L301，EOF while reading ECP pointer card.]
 * [L301，No solvent atoms in DisRep.]
 * [L301，Atomic number out of range for XXX basis set.]
 * [L301，R6DS8: Unable to choose the S8 parameter]
 * [L301，R6DRCv: No RCov radius available for IA=XX]
 * [L301，R6DC6: No C6 coefficient available for IA=XX]
 * [L502，Convergence failure]
 * [L502，Inaccurate quadrature in CalDSu.]
 * [L502，Inv3 failed in PCMMkU]
 * [L508，Convergence failure]
 * [L508，Inv3 failed in PCMMkU]
 * [L602，GetVDW:  no radius for atom XX atomic number XX.]
 * [L801，Excessive mixing of core and valence orbitals.]
 * [L801, Fatal Problem: The smallest alpha delta epsilon is XXXXXX]
 * [L913，\*MAX. CYCLES\*]
 * [L914，XXXXXX words are not enough for AIAXAO.]
 * [L1002，Inaccurate quadrature in CalDSu.]
 * [L1002，No func 3rd derivs with XXX.]
 * [L1002，NIJ > Max2 in MMCore.]
 * [L1002，XXXXXX words are not enough for AIAXAO.]
 * [L9999，Optimization stopped.]
### Computer/OS related errors
#### CPU
 * [Error: illegal instruction, illegal opcode]
#### File
 * [Internal input file was deleted!]
 * [open-new-file]
 * [Error Message # 2066. Can't create file Temp input file 'gxx.inp']
#### Hard drive
 * [Erroneous write]
 * [g_write]
#### Memory
 * [needs more words of memory]
 * [Not enough memory to run at all]
 * [Out-of-memory error in routine XXX]
 * [galloc:  could not allocate memory.]
### Difficult cases
 * [NtrErr Called from XXXXXX.]
### Probably known bugs
 * [Gaussian Bug 的“样式”及发现Bug后的可能做法]
 * [L103，Bad arguments to LAPack or BLAS routine.]
 * [L401，Diagonalization in DiagDN via DSPEV failed.]
 * [L906，Internal consistency failure #1 in GetIJB.]
 * [L914，Unable to match L and R vectors in BiOrth]
 * [L1002，NIJ > Max2 in MMCore.]
 * [L1014，Tx not orthogonal to T]
### Abnormal situations that doesn't give an error message
 * [IRC提前停止或折返]
 * [优化后的结构有一个或几个小虚频]
 * [G09 Windows 在 L1.exe 左右无报错退出]
 * [GaussView观看结构有异常的成键、断键]
 * [GaussView 中显示的 IRC 在零点附近出现异常的低能点]
### Other common entry-level questions
 * [GaussView 打开 chk 或 fchk 文件报错 Missing or bad data: Alpha Orbital Energies]
 * [“这种计算大约需多长时间？”]
 * [如何通过柔性扫描产生较好的过渡态初猜]
 * [如何在量化计算中设定原子/片段的电荷]
 * [如何计算 Activation Strain (Distortion-Interaction) Energy]

## Explanation and solution for the errors
For ones who would like to read this in whole, the order of the following sections is different from the [list of errors](#List-of-errors) above. Use the anchor links if you would like to navigate to specific errors.

### General errors
<a name="SevereErrorMessage2070"></a>
####  · Severe Error Message # 2070 (Windows)
####  · segmentation violation/segmentation fault (Linux)
#
### QM related errors

####  · L502，Convergence failure
#
####  · L508，Convergence failure
#
####  · L502/L1002，Inaccurate quadrature in CalDSu.
#
####  · L9999，Optimization stopped.
#
####  · L123，Max corrector steps exceded
####  · L123，GS2 Optimization Failure.
#
####  · L103，Error in internal coordinate system
####  · L103，Linear angle in Bend; Linear angle in Tors
####  · L103，FormBX had a problem
#
####  · L101，End of file in ZSymb.
####  · L301，End of file reading basis center.
####  · L301，EOF while reading ECP pointer card.
#
####  · L101，WANTED A XXX AS INPUT. FOUND AN XXX AS INPUT.
#
####  · L101，Input Error Input Error Input Error Input Error Input Error Input Error
#
####  · L202，Problem with the distance matrix.
####  · L202，Atoms too close.
#
####  · L1，Illegal IType or MSType generated by parse.
#
####  · L1，ntrex1
#
####  · L1，QPErr --- A syntax error was detected in the input line.
#
####  · L301，Atomic number out of range for XXX basis set.
#
####  · L301，The combination of multiplicity X and XXX electrons is impossible.
#
####  · L301，R6DS8: Unable to choose the S8 parameter
#
####  · L301，R6DRCv: No RCov radius available for IA=XX
####  · L301，R6DC6: No C6 coefficient available for IA=XX
#
####  · L114，ERROR IN INITNF. NUMBER OF VARIABLES (  0) INCORRECT (SHOULD BE BETWEEN 1 AND 50)
#
####  · L801，Excessive mixing of core and valence orbitals.
#
####  · L801, Fatal Problem: The smallest alpha delta epsilon is XXXXXX
#
####  · L502/L508，Inv3 failed in PCMMkU
#
####  · L913，\*MAX. CYCLES\*
#
####  · L103，New curvilinear step not converged. Error imposing constraints.
#
####  · L301，No solvent atoms in DisRep.
#
####  · L103，NRF ne Abs NRFX
#
####  · L123，GetHes: LRWHes > LHess!
#
####  · L1002，No func 3rd derivs with XXX.
#
####  · L602，GetVDW:  no radius for atom XX atomic number XX.
#

### Computer/OS related errors
####  · Error: illegal instruction, illegal opcode
#
####  · Internal input file was deleted!
#
####  · open-new-file
#
####  · Error Message # 2066. Can't create file Temp input file 'gxx.inp'
#
####  · Erroneous write
####  · g_write
#
####  · L914，XXXXXX words are not enough for AIAXAO.
####  · L1002，XXXXXX words are not enough for AIAXAO.
####  · needs more words of memory
####  · Not enough memory to run at all
####  · Out-of-memory error in routine XXX
#
####  · galloc:  could not allocate memory.
#
### Difficult cases
####  · NtrErr Called from XXXXXX.
#
### Probably known bugs
####  · Gaussian Bug 的“样式”及发现Bug后的可能做法
Some known bugs:
 * L103，Bad arguments to LAPack or BLAS routine.
 * L401，Diagonalization in DiagDN via DSPEV failed.
 * L906，Internal consistency failure #1 in GetIJB.
 * L914，Unable to match L and R vectors in BiOrth
 * L1002，NIJ > Max2 in MMCore.
 * L1014，Tx not orthogonal to T
#
### Abnormal situations that doesn't give an error message
####  · IRC提前停止或折返
#
####  · 优化后的结构有一个或几个小虚频
#
####  · G09 Windows 在 L1.exe 左右无报错退出
#
####  · GaussView观看结构有异常的成键、断键
#
####  · GaussView 中显示的 IRC 在零点附近出现异常的低能点
#
####  · GaussView 打开 chk 或 fchk 文件报错 Missing or bad data: Alpha Orbital Energies
#
### Other common entry-level questions
####  · “这种计算大约需多长时间？”
#
####  · 如何通过柔性扫描产生较好的过渡态初猜
#
####  · 如何在量化计算中设定原子/片段的电荷
#
####  · 如何计算 Activation Strain (Distortion-Interaction) Energy
#

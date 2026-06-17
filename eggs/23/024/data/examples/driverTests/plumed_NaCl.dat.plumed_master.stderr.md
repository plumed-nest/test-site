**Project ID:** [plumID:23.024]({{ '/' | absolute_url }}eggs/23/024/)  
Stderr for source:  examples/driverTests/plumed_NaCl.dat   
Download: [zipped raw stdout](plumed_NaCl.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_NaCl.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../../src/pines/PINES.w1PF4c.cpp: In static member function ‘static void PLMD::PINES::PINES::registerKeywords(PLMD::Keywords&)’:
../../src/pines/PINES.w1PF4c.cpp:158:3: error: ‘componentsAreNotOptional’ was not declared in this scope
158 |   componentsAreNotOptional(keys);
|   ^~~~~~~~~~~~~~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:160:26: warning: ‘void PLMD::Keywords::addOutputComponent(const std::string&, const std::string&, const std::string&)’ is deprecated: Use addOutputComponent with four argument and specify valid types for value from scalar/vector/matrix/grid [-Wdeprecated-declarations]
160 |   keys.addOutputComponent("ELEMENT", "default", "Elements of the PINES block. The position in the N choose 2 interactions (i) and the neighbor in the neighbor list (j) is given as PINES-i-j.");
|   ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:28,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from ../../src/pines/PINES.w1PF4c.cpp:17:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/Keywords.h:268:8: note: declared here
268 |   void addOutputComponent( const std::string& name, const std::string& key, const std::string& descr );
|        ^~~~~~~~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp: In constructor ‘PLMD::PINES::PINES::PINES(const PLMD::ActionOptions&)’:
../../src/pines/PINES.w1PF4c.cpp:356:69: warning: ‘bool PLMD::PlumedMain::DeprecatedAtoms::usingNaturalUnits() const’ is deprecated: Use Action::usingNaturalUnits(). [-Wdeprecated-declarations]
356 |     mypdb.readFromFilepointer(fp,plumed.getAtoms().usingNaturalUnits(),0.1/atoms.getUnits().getLength());
|                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~
In file included from ../../src/pines/PINES.w1PF4c.cpp:19:
/home/runner/opt/include/plumed_master/core/PlumedMain.h:108:10: note: declared here
108 |     bool usingNaturalUnits() const ;
|          ^~~~~~~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:356:76: error: ‘atoms’ was not declared in this scope; did you mean ‘Atoms’?
356 |     mypdb.readFromFilepointer(fp,plumed.getAtoms().usingNaturalUnits(),0.1/atoms.getUnits().getLength());
|                                                                            ^~~~~
|                                                                            Atoms
../../src/pines/PINES.w1PF4c.cpp:379:14: warning: comparison of integer expressions of different signedness: ‘int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<unsigned int>, unsigned int>::value_type’ {aka ‘unsigned int’} [-Wsign-compare]
379 |       if(rind==Presind[j]) {
../../src/pines/PINES.w1PF4c.cpp:416:11: warning: unused variable ‘rind’ [-Wunused-variable]
416 |       int rind=mypdb.getResidueNumber(anum);
|           ^~~~
../../src/pines/PINES.w1PF4c.cpp:1012:21: warning: comparison of integer expressions of different signedness: ‘int’ and ‘std::vector<std::vector<PLMD::VectorTyped<double, 3> > >::size_type’ {aka ‘long unsigned int’} [-Wsign-compare]
1012 |   for (int i = 0; i < ann_deriv.size(); i++) {
|                   ~~^~~~~~~~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp: In member function ‘virtual void PLMD::PINES::PINES::prepare()’:
../../src/pines/PINES.w1PF4c.cpp:1090:11: warning: unused variable ‘buffer’ [-Wunused-variable]
1090 |       int buffer=10;
|           ^~~~~~
../../src/pines/PINES.w1PF4c.cpp: In member function ‘virtual void PLMD::PINES::PINES::calculate()’:
../../src/pines/PINES.w1PF4c.cpp:1337:12: error: invalid use of incomplete type ‘class PLMD::Communicator’
1337 |     stride=comm.Get_size();
|            ^~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/OFile.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Log.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:31:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1338:10: error: invalid use of incomplete type ‘class PLMD::Communicator’
1338 |     rank=comm.Get_rank();
|          ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1512:27: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
1512 |               if(sb_count > max_solv_atoms) {
|                  ~~~~~~~~~^~~~~~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1567:34: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
1567 |           if(nl_small[j]->size() >= max_solv_atoms) {
|              ~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1575:44: warning: comparison of integer expressions of different signedness: ‘std::vector<int>::size_type’ {aka ‘long unsigned int’} and ‘int’ [-Wsign-compare]
1575 |                 if(sb_count - A0[i].size() < max_solv_atoms) {
|                    ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1589:25: error: invalid use of incomplete type ‘class PLMD::Communicator’
1589 |         if(!doserial && comm.initialized()) {
|                         ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1620:11: error: invalid use of incomplete type ‘class PLMD::Communicator’
1620 |           comm.Barrier();
|           ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1625:11: error: invalid use of incomplete type ‘class PLMD::Communicator’
1625 |           comm.Allgather(&dim,1,&Vdim[0],1);
|           ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1640:11: error: invalid use of incomplete type ‘class PLMD::Communicator’
1640 |           comm.Allgather(&OrdVec[0],Nprec,&OrdVecAll[0],Nprec);
|           ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1642:11: error: invalid use of incomplete type ‘class PLMD::Communicator’
1642 |           comm.Allgatherv(&Atom0F[0],Atom0F.size(),&Atom0FAll[0],&Vdim[0],&Vpos[0]);
|           ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1643:11: error: invalid use of incomplete type ‘class PLMD::Communicator’
1643 |           comm.Allgatherv(&Atom1F[0],Atom1F.size(),&Atom1FAll[0],&Vdim[0],&Vpos[0]);
|           ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1656:34: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
1656 |               for(unsigned m=0; m<OrdVecAll[i+l*Nprec]; m++) {
../../src/pines/PINES.w1PF4c.cpp:1668:32: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
1668 |             for(unsigned m=0; m<OrdVec[i]; m++) {
../../src/pines/PINES.w1PF4c.cpp:1723:18: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
1723 |         if(limit > max_solv_atoms) {
|            ~~~~~~^~~~~~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1704:10: warning: unused variable ‘dosorting’ [-Wunused-variable]
1704 |     bool dosorting=dosort[j];
|          ^~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1801:18: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
1801 |         if(limit > max_solv_atoms) {
|            ~~~~~~^~~~~~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1826:16: warning: unused variable ‘tPINES’ [-Wunused-variable]
1826 |         double tPINES = sfs[j].calculate(dm*Fvol, dfunc);
|                ^~~~~~
../../src/pines/PINES.w1PF4c.cpp:1848:20: error: invalid use of incomplete type ‘class PLMD::Communicator’
1848 |     if (!serial && comm.initialized() ) {
|                    ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1856:7: error: invalid use of incomplete type ‘class PLMD::Communicator’
1856 |       comm.Barrier();
|       ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1860:11: error: invalid use of incomplete type ‘class PLMD::Communicator’
1860 |           comm.Sum(cPINES[j][k]);
|           ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1861:27: error: invalid use of incomplete type ‘class PLMD::Communicator’
1861 |           cPINES[j][k] /= comm.Get_size();
|                           ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1870:15: error: invalid use of incomplete type ‘class PLMD::Communicator’
1870 |               comm.Sum(ann_deriv[i][j][k]);
|               ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1871:37: error: invalid use of incomplete type ‘class PLMD::Communicator’
1871 |               ann_deriv[i][j][k] /= comm.Get_size();
|                                     ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1877:7: error: invalid use of incomplete type ‘class PLMD::Communicator’
1877 |       comm.Sum(&m_virial[0][0],9);
|       ^~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/FileBase.h:29:7: note: forward declaration of ‘class PLMD::Communicator’
29 | class Communicator;
|       ^~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1902:18: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
1902 |       if( (limit > max_solv_atoms) && (solv_blocks != 0) ){
|            ~~~~~~^~~~~~~~~~~~~~~~
../../src/pines/PINES.w1PF4c.cpp:1771:8: warning: unused variable ‘Nder’ [-Wunused-variable]
1771 |   bool Nder=CompDer;
|        ^~~~
../../src/pines/PINES.w1PF4c.cpp:1772:8: warning: unused variable ‘Scalevol’ [-Wunused-variable]
1772 |   bool Scalevol=Svol;
|        ^~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../src/pines/PINES.2.11.0-dev.so ../../src/pines/PINES.cpp

[runnervm1li68:07020] *** Process received signal ***
[runnervm1li68:07020] Signal: Aborted (6)
[runnervm1li68:07020] Signal code:  (-6)
[runnervm1li68:07020] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7efc47845330]
[runnervm1li68:07020] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7efc4789eb2c]
[runnervm1li68:07020] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7efc4784527e]
[runnervm1li68:07020] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7efc478288ff]
[runnervm1li68:07020] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7efc47ca5ff5]
[runnervm1li68:07020] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7efc47cbb0da]
[runnervm1li68:07020] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7efc47ca5a55]
[runnervm1li68:07020] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7efc47ca5a6f]
[runnervm1li68:07020] [ 8] plumed_master(+0x146dd)[0x55e7f17346dd]
[runnervm1li68:07020] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7efc4782a1ca]
[runnervm1li68:07020] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7efc4782a28b]
[runnervm1li68:07020] [11] plumed_master(+0x15365)[0x55e7f1735365]
[runnervm1li68:07020] *** End of error message ***
</pre>
{% endraw %}

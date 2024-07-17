**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
Stderr for source:  CO2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../codes/StructureFactor_descriptor.test.0Psi09.cpp: In constructor ‘PLMD::colvar::StructureFactor_descriptor_test::StructureFactor_descriptor_test(const PLMD::ActionOptions&)’:
../codes/StructureFactor_descriptor.test.0Psi09.cpp:188:41: warning: ‘int PLMD::PlumedMain::DeprecatedAtoms::getNatoms() const’ is deprecated [-Wdeprecated-declarations]
188 |     NumAtom_=plumed.getAtoms().getNatoms();
|              ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~
In file included from ../codes/StructureFactor_descriptor.test.0Psi09.cpp:8:
/home/runner/opt/include/plumed_master/core/PlumedMain.h:107:9: note: declared here
107 |     int getNatoms() const ;
|         ^~~~~~~~~
../codes/StructureFactor_descriptor.test.0Psi09.cpp:194:108: warning: ‘int PLMD::PlumedMain::DeprecatedAtoms::getNatoms() const’ is deprecated [-Wdeprecated-declarations]
194 |   log.printf("  over a total of N_tot=%d, considering a number of atoms N=%d\n",plumed.getAtoms().getNatoms(),NumAtom_);
|                                                                                 ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~
In file included from ../codes/StructureFactor_descriptor.test.0Psi09.cpp:8:
/home/runner/opt/include/plumed_master/core/PlumedMain.h:107:9: note: declared here
107 |     int getNatoms() const ;
|         ^~~~~~~~~
Assembler messages:
Fatal error: can't create plumed_mklib.rBmN75/../codes/StructureFactor_descriptor.test.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1292) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../codes/StructureFactor_descriptor.test.2.10.0-dev.so ../codes/StructureFactor_descriptor.test.cpp

[fv-az1108-41:73405] *** Process received signal ***
[fv-az1108-41:73405] Signal: Aborted (6)
[fv-az1108-41:73405] Signal code:  (-6)
[fv-az1108-41:73405] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f438be42520]
[fv-az1108-41:73405] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f438be969fc]
[fv-az1108-41:73405] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f438be42476]
[fv-az1108-41:73405] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f438be287f3]
[fv-az1108-41:73405] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f438c2a2b9e]
[fv-az1108-41:73405] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f438c2ae20c]
[fv-az1108-41:73405] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f438c2ae277]
[fv-az1108-41:73405] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f438c2ae52b]
[fv-az1108-41:73405] [ 8] plumed_master(+0x14274)[0x55cd62143274]
[fv-az1108-41:73405] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f438be29d90]
[fv-az1108-41:73405] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f438be29e40]
[fv-az1108-41:73405] [11] plumed_master(+0x14ed5)[0x55cd62143ed5]
[fv-az1108-41:73405] *** End of error message ***
</pre>
{% endraw %}

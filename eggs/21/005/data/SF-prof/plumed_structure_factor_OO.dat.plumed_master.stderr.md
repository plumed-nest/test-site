**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
Stderr for source:  SF-prof/plumed_structure_factor_OO.dat   
Download: [zipped raw stdout](plumed_structure_factor_OO.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_structure_factor_OO.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../codes/StructureFactor_sphericallyAveraged.MCDZiS.cpp: In constructor ‘PLMD::colvar::StructureFactor_sphericallyAveraged::StructureFactor_sphericallyAveraged(const PLMD::ActionOptions&)’:
../codes/StructureFactor_sphericallyAveraged.MCDZiS.cpp:184:41: warning: ‘int PLMD::PlumedMain::DeprecatedAtoms::getNatoms() const’ is deprecated [-Wdeprecated-declarations]
184 |     NumAtom_=plumed.getAtoms().getNatoms();
|              ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~
In file included from ../codes/StructureFactor_sphericallyAveraged.MCDZiS.cpp:8:
/home/runner/opt/include/plumed_master/core/PlumedMain.h:107:9: note: declared here
107 |     int getNatoms() const ;
|         ^~~~~~~~~
../codes/StructureFactor_sphericallyAveraged.MCDZiS.cpp:190:108: warning: ‘int PLMD::PlumedMain::DeprecatedAtoms::getNatoms() const’ is deprecated [-Wdeprecated-declarations]
190 |   log.printf("  over a total of N_tot=%d, considering a number of atoms N=%d\n",plumed.getAtoms().getNatoms(),NumAtom_);
|                                                                                 ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~
In file included from ../codes/StructureFactor_sphericallyAveraged.MCDZiS.cpp:8:
/home/runner/opt/include/plumed_master/core/PlumedMain.h:107:9: note: declared here
107 |     int getNatoms() const ;
|         ^~~~~~~~~
Assembler messages:
Fatal error: can't create plumed_mklib.RvuTLR/../codes/StructureFactor_sphericallyAveraged.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1292) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../codes/StructureFactor_sphericallyAveraged.2.10.0-dev.so ../codes/StructureFactor_sphericallyAveraged.cpp

[fv-az1108-41:73526] *** Process received signal ***
[fv-az1108-41:73526] Signal: Aborted (6)
[fv-az1108-41:73526] Signal code:  (-6)
[fv-az1108-41:73526] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4ce7842520]
[fv-az1108-41:73526] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4ce78969fc]
[fv-az1108-41:73526] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4ce7842476]
[fv-az1108-41:73526] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4ce78287f3]
[fv-az1108-41:73526] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f4ce7ca2b9e]
[fv-az1108-41:73526] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f4ce7cae20c]
[fv-az1108-41:73526] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f4ce7cae277]
[fv-az1108-41:73526] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4ce7cae52b]
[fv-az1108-41:73526] [ 8] plumed_master(+0x14274)[0x55a865aa8274]
[fv-az1108-41:73526] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4ce7829d90]
[fv-az1108-41:73526] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4ce7829e40]
[fv-az1108-41:73526] [11] plumed_master(+0x14ed5)[0x55a865aa8ed5]
[fv-az1108-41:73526] *** End of error message ***
</pre>
{% endraw %}

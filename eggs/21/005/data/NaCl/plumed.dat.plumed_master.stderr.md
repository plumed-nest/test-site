**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
Stderr for source:  NaCl/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../codes/StructureFactor_descriptor.test.k2MclO.cpp: In constructor ‘PLMD::colvar::StructureFactor_descriptor_test::StructureFactor_descriptor_test(const PLMD::ActionOptions&)’:
../codes/StructureFactor_descriptor.test.k2MclO.cpp:188:21: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
188 |     NumAtom_=plumed.getAtoms().getNatoms();
|                     ^~~~~~~~
../codes/StructureFactor_descriptor.test.k2MclO.cpp:194:88: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
194 |   log.printf("  over a total of N_tot=%d, considering a number of atoms N=%d\n",plumed.getAtoms().getNatoms(),NumAtom_);
|                                                                                        ^~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../codes/StructureFactor_descriptor.test.cpp

[fv-az695-903:07881] *** Process received signal ***
[fv-az695-903:07881] Signal: Aborted (6)
[fv-az695-903:07881] Signal code:  (-6)
[fv-az695-903:07881] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1c32642520]
[fv-az695-903:07881] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1c326969fc]
[fv-az695-903:07881] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1c32642476]
[fv-az695-903:07881] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1c326287f3]
[fv-az695-903:07881] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f1c32aa4f26]
[fv-az695-903:07881] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f1c32ab6d9c]
[fv-az695-903:07881] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f1c32ab6e07]
[fv-az695-903:07881] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1c32ab70bb]
[fv-az695-903:07881] [ 8] plumed_master(+0x12ebf)[0x557fe6466ebf]
[fv-az695-903:07881] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1c32629d90]
[fv-az695-903:07881] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1c32629e40]
[fv-az695-903:07881] [11] plumed_master(+0x13155)[0x557fe6467155]
[fv-az695-903:07881] *** End of error message ***
</pre>
{% endraw %}

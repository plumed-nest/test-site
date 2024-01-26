**Project ID:** [plumID:21.039]({{ '/' | absolute_url }}eggs/21/039/)  
Stderr for source:  data/silicon/1_opes_dlda/plumed-driver.dat   
Download: [zipped raw stdout](plumed-driver.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-driver.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../StructureFactor_descriptor.test.XDNSUo.cpp: In constructor ‘PLMD::colvar::StructureFactor_descriptor_test::StructureFactor_descriptor_test(const PLMD::ActionOptions&)’:
../StructureFactor_descriptor.test.XDNSUo.cpp:223:21: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
223 |     NumAtom_=plumed.getAtoms().getNatoms();
|                     ^~~~~~~~
../StructureFactor_descriptor.test.XDNSUo.cpp:229:88: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
229 |   log.printf("  over a total of N_tot=%d, considering a number of atoms N=%d\n",plumed.getAtoms().getNatoms(),NumAtom_);
|                                                                                        ^~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../StructureFactor_descriptor.test.cpp

[fv-az532-512:09072] *** Process received signal ***
[fv-az532-512:09072] Signal: Aborted (6)
[fv-az532-512:09072] Signal code:  (-6)
[fv-az532-512:09072] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe7b3c42520]
[fv-az532-512:09072] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe7b3c969fc]
[fv-az532-512:09072] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe7b3c42476]
[fv-az532-512:09072] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe7b3c287f3]
[fv-az532-512:09072] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fe7b40a4f26]
[fv-az532-512:09072] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fe7b40b6d9c]
[fv-az532-512:09072] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fe7b40b6e07]
[fv-az532-512:09072] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe7b40b70bb]
[fv-az532-512:09072] [ 8] plumed_master(+0x12ebf)[0x55a16c3b9ebf]
[fv-az532-512:09072] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe7b3c29d90]
[fv-az532-512:09072] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe7b3c29e40]
[fv-az532-512:09072] [11] plumed_master(+0x13155)[0x55a16c3ba155]
[fv-az532-512:09072] *** End of error message ***
</pre>
{% endraw %}

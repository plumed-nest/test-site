**Project ID:** [plumID:21.039]({{ '/' | absolute_url }}eggs/21/039/)  
Stderr for source:  data/silicon/1_opes_dlda/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../StructureFactor_descriptor.test.7ci1jJ.cpp: In constructor ‘PLMD::colvar::StructureFactor_descriptor_test::StructureFactor_descriptor_test(const PLMD::ActionOptions&)’:
../StructureFactor_descriptor.test.7ci1jJ.cpp:223:21: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
223 |     NumAtom_=plumed.getAtoms().getNatoms();
|                     ^~~~~~~~
../StructureFactor_descriptor.test.7ci1jJ.cpp:229:88: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
229 |   log.printf("  over a total of N_tot=%d, considering a number of atoms N=%d\n",plumed.getAtoms().getNatoms(),NumAtom_);
|                                                                                        ^~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../StructureFactor_descriptor.test.cpp

[fv-az532-512:09129] *** Process received signal ***
[fv-az532-512:09129] Signal: Aborted (6)
[fv-az532-512:09129] Signal code:  (-6)
[fv-az532-512:09129] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb707842520]
[fv-az532-512:09129] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb7078969fc]
[fv-az532-512:09129] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb707842476]
[fv-az532-512:09129] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb7078287f3]
[fv-az532-512:09129] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fb707ca4f26]
[fv-az532-512:09129] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fb707cb6d9c]
[fv-az532-512:09129] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fb707cb6e07]
[fv-az532-512:09129] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb707cb70bb]
[fv-az532-512:09129] [ 8] plumed_master(+0x12ebf)[0x558424adfebf]
[fv-az532-512:09129] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb707829d90]
[fv-az532-512:09129] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb707829e40]
[fv-az532-512:09129] [11] plumed_master(+0x13155)[0x558424ae0155]
[fv-az532-512:09129] *** End of error message ***
</pre>
{% endraw %}

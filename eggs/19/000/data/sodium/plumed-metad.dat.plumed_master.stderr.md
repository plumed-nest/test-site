**Project ID:** [plumID:19.000]({{ '/' | absolute_url }}eggs/19/000/)  
Stderr for source:  sodium/plumed-metad.dat   
Download: [zipped raw stdout](plumed-metad.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-metad.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
DebyeStructureFactor.J47rkW.cpp: In constructor ‘PLMD::colvar::DebyeStructureFactor::DebyeStructureFactor(const PLMD::ActionOptions&)’:
DebyeStructureFactor.J47rkW.cpp:287:21: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
287 |     NumAtom_=plumed.getAtoms().getNatoms();
|                     ^~~~~~~~
DebyeStructureFactor.J47rkW.cpp:341:88: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
341 |   log.printf("  over a total of N_tot=%d, considering a number of atoms N=%d\n",plumed.getAtoms().getNatoms(),NumAtom_);
|                                                                                        ^~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh DebyeStructureFactor.cpp

[fv-az979-741:09662] *** Process received signal ***
[fv-az979-741:09662] Signal: Aborted (6)
[fv-az979-741:09662] Signal code:  (-6)
[fv-az979-741:09662] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa2c9642520]
[fv-az979-741:09662] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa2c96969fc]
[fv-az979-741:09662] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa2c9642476]
[fv-az979-741:09662] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa2c96287f3]
[fv-az979-741:09662] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fa2c9aa4f26]
[fv-az979-741:09662] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fa2c9ab6d9c]
[fv-az979-741:09662] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fa2c9ab6e07]
[fv-az979-741:09662] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa2c9ab70bb]
[fv-az979-741:09662] [ 8] plumed_master(+0x12ebf)[0x55cd48fe6ebf]
[fv-az979-741:09662] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa2c9629d90]
[fv-az979-741:09662] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa2c9629e40]
[fv-az979-741:09662] [11] plumed_master(+0x13155)[0x55cd48fe7155]
[fv-az979-741:09662] *** End of error message ***
</pre>
{% endraw %}

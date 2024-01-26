**Project ID:** [plumID:19.000]({{ '/' | absolute_url }}eggs/19/000/)  
Stderr for source:  sodium/plumed-ves.dat   
Download: [zipped raw stdout](plumed-ves.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-ves.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
DebyeStructureFactor.ILa0Sq.cpp: In constructor ‘PLMD::colvar::DebyeStructureFactor::DebyeStructureFactor(const PLMD::ActionOptions&)’:
DebyeStructureFactor.ILa0Sq.cpp:287:21: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
287 |     NumAtom_=plumed.getAtoms().getNatoms();
|                     ^~~~~~~~
DebyeStructureFactor.ILa0Sq.cpp:341:88: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
341 |   log.printf("  over a total of N_tot=%d, considering a number of atoms N=%d\n",plumed.getAtoms().getNatoms(),NumAtom_);
|                                                                                        ^~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh DebyeStructureFactor.cpp

[fv-az979-741:09718] *** Process received signal ***
[fv-az979-741:09718] Signal: Aborted (6)
[fv-az979-741:09718] Signal code:  (-6)
[fv-az979-741:09718] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd2a7e42520]
[fv-az979-741:09718] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd2a7e969fc]
[fv-az979-741:09718] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd2a7e42476]
[fv-az979-741:09718] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd2a7e287f3]
[fv-az979-741:09718] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fd2a82a4f26]
[fv-az979-741:09718] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fd2a82b6d9c]
[fv-az979-741:09718] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fd2a82b6e07]
[fv-az979-741:09718] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd2a82b70bb]
[fv-az979-741:09718] [ 8] plumed_master(+0x12ebf)[0x5592cdee2ebf]
[fv-az979-741:09718] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd2a7e29d90]
[fv-az979-741:09718] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd2a7e29e40]
[fv-az979-741:09718] [11] plumed_master(+0x13155)[0x5592cdee3155]
[fv-az979-741:09718] *** End of error message ***
</pre>
{% endraw %}

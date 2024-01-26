**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
Stderr for source:  SF-prof/plumed_structure_factor_OO.dat   
Download: [zipped raw stdout](plumed_structure_factor_OO.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_structure_factor_OO.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../codes/StructureFactor_sphericallyAveraged.U6DHtX.cpp: In constructor ‘PLMD::colvar::StructureFactor_sphericallyAveraged::StructureFactor_sphericallyAveraged(const PLMD::ActionOptions&)’:
../codes/StructureFactor_sphericallyAveraged.U6DHtX.cpp:184:21: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
184 |     NumAtom_=plumed.getAtoms().getNatoms();
|                     ^~~~~~~~
../codes/StructureFactor_sphericallyAveraged.U6DHtX.cpp:190:88: error: ‘class PLMD::PlumedMain’ has no member named ‘getAtoms’
190 |   log.printf("  over a total of N_tot=%d, considering a number of atoms N=%d\n",plumed.getAtoms().getNatoms(),NumAtom_);
|                                                                                        ^~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../codes/StructureFactor_sphericallyAveraged.cpp

[fv-az695-903:07937] *** Process received signal ***
[fv-az695-903:07937] Signal: Aborted (6)
[fv-az695-903:07937] Signal code:  (-6)
[fv-az695-903:07937] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f321ea42520]
[fv-az695-903:07937] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f321ea969fc]
[fv-az695-903:07937] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f321ea42476]
[fv-az695-903:07937] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f321ea287f3]
[fv-az695-903:07937] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f321eea4f26]
[fv-az695-903:07937] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f321eeb6d9c]
[fv-az695-903:07937] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f321eeb6e07]
[fv-az695-903:07937] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f321eeb70bb]
[fv-az695-903:07937] [ 8] plumed_master(+0x12ebf)[0x564d935b4ebf]
[fv-az695-903:07937] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f321ea29d90]
[fv-az695-903:07937] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f321ea29e40]
[fv-az695-903:07937] [11] plumed_master(+0x13155)[0x564d935b5155]
[fv-az695-903:07937] *** End of error message ***
</pre>
{% endraw %}

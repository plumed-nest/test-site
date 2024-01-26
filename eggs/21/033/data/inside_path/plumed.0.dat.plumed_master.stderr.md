**Project ID:** [plumID:21.033]({{ '/' | absolute_url }}eggs/21/033/)  
Stderr for source:  inside_path/plumed.0.dat   
Download: [zipped raw stdout](plumed.0.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.0.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../PathCV.GSYBr1.cpp:25:10: fatal error: core/Atoms.h: No such file or directory
25 | #include "core/Atoms.h"
|          ^~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../PathCV.cpp

[fv-az1148-6:06579] *** Process received signal ***
[fv-az1148-6:06579] Signal: Aborted (6)
[fv-az1148-6:06579] Signal code:  (-6)
[fv-az1148-6:06579] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3933e42520]
[fv-az1148-6:06579] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3933e969fc]
[fv-az1148-6:06579] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3933e42476]
[fv-az1148-6:06579] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3933e287f3]
[fv-az1148-6:06579] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f39342a4f26]
[fv-az1148-6:06579] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f39342b6d9c]
[fv-az1148-6:06579] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f39342b6e07]
[fv-az1148-6:06579] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f39342b70bb]
[fv-az1148-6:06579] [ 8] plumed_master(+0x12ebf)[0x55a1d13b4ebf]
[fv-az1148-6:06579] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3933e29d90]
[fv-az1148-6:06579] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3933e29e40]
[fv-az1148-6:06579] [11] plumed_master(+0x13155)[0x55a1d13b5155]
[fv-az1148-6:06579] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:22.002]({{ '/' | absolute_url }}eggs/22/002/)  
Stderr for source:  OAH-G1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
GAMBES_log_static_few.PTMUMs.cpp:23:10: fatal error: core/Atoms.h: No such file or directory
23 | #include "core/Atoms.h"
|          ^~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh GAMBES_log_static_few.cpp

[fv-az695-903:05752] *** Process received signal ***
[fv-az695-903:05752] Signal: Aborted (6)
[fv-az695-903:05752] Signal code:  (-6)
[fv-az695-903:05752] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fab49e42520]
[fv-az695-903:05752] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fab49e969fc]
[fv-az695-903:05752] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fab49e42476]
[fv-az695-903:05752] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fab49e287f3]
[fv-az695-903:05752] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fab4a2a4f26]
[fv-az695-903:05752] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fab4a2b6d9c]
[fv-az695-903:05752] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fab4a2b6e07]
[fv-az695-903:05752] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fab4a2b70bb]
[fv-az695-903:05752] [ 8] plumed_master(+0x12ebf)[0x55ba650f6ebf]
[fv-az695-903:05752] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fab49e29d90]
[fv-az695-903:05752] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fab49e29e40]
[fv-az695-903:05752] [11] plumed_master(+0x13155)[0x55ba650f7155]
[fv-az695-903:05752] *** End of error message ***
</pre>
{% endraw %}

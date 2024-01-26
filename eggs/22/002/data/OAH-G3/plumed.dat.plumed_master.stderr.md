**Project ID:** [plumID:22.002]({{ '/' | absolute_url }}eggs/22/002/)  
Stderr for source:  OAH-G3/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
GAMBES_log.lCN7ZM.cpp:23:10: fatal error: core/Atoms.h: No such file or directory
23 | #include "core/Atoms.h"
|          ^~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh GAMBES_log.cpp

[fv-az695-903:05939] *** Process received signal ***
[fv-az695-903:05939] Signal: Aborted (6)
[fv-az695-903:05939] Signal code:  (-6)
[fv-az695-903:05939] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb6eb242520]
[fv-az695-903:05939] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb6eb2969fc]
[fv-az695-903:05939] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb6eb242476]
[fv-az695-903:05939] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb6eb2287f3]
[fv-az695-903:05939] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fb6eb6a4f26]
[fv-az695-903:05939] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fb6eb6b6d9c]
[fv-az695-903:05939] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fb6eb6b6e07]
[fv-az695-903:05939] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb6eb6b70bb]
[fv-az695-903:05939] [ 8] plumed_master(+0x12ebf)[0x555c7775febf]
[fv-az695-903:05939] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb6eb229d90]
[fv-az695-903:05939] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb6eb229e40]
[fv-az695-903:05939] [11] plumed_master(+0x13155)[0x555c77760155]
[fv-az695-903:05939] *** End of error message ***
</pre>
{% endraw %}

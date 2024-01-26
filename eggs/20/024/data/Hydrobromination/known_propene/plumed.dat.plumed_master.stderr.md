**Project ID:** [plumID:20.024]({{ '/' | absolute_url }}eggs/20/024/)  
Stderr for source:  Hydrobromination/known_propene/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../../GAMBES.l0Zkdz.cpp:23:10: fatal error: core/Atoms.h: No such file or directory
23 | #include "core/Atoms.h"
|          ^~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../../GAMBES.cpp

[fv-az532-512:09994] *** Process received signal ***
[fv-az532-512:09994] Signal: Aborted (6)
[fv-az532-512:09994] Signal code:  (-6)
[fv-az532-512:09994] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f94e2a42520]
[fv-az532-512:09994] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f94e2a969fc]
[fv-az532-512:09994] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f94e2a42476]
[fv-az532-512:09994] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f94e2a287f3]
[fv-az532-512:09994] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f94e2ea4f26]
[fv-az532-512:09994] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f94e2eb6d9c]
[fv-az532-512:09994] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f94e2eb6e07]
[fv-az532-512:09994] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f94e2eb70bb]
[fv-az532-512:09994] [ 8] plumed_master(+0x12ebf)[0x55ed49e82ebf]
[fv-az532-512:09994] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f94e2a29d90]
[fv-az532-512:09994] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f94e2a29e40]
[fv-az532-512:09994] [11] plumed_master(+0x13155)[0x55ed49e83155]
[fv-az532-512:09994] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:20.024]({{ '/' | absolute_url }}eggs/20/024/)  
Stderr for source:  Alanine-dipeptide/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../GAMBES.l6nK7M.cpp:23:10: fatal error: core/Atoms.h: No such file or directory
23 | #include "core/Atoms.h"
|          ^~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../GAMBES.cpp

[fv-az532-512:09878] *** Process received signal ***
[fv-az532-512:09878] Signal: Aborted (6)
[fv-az532-512:09878] Signal code:  (-6)
[fv-az532-512:09878] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f60b1442520]
[fv-az532-512:09878] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f60b14969fc]
[fv-az532-512:09878] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f60b1442476]
[fv-az532-512:09878] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f60b14287f3]
[fv-az532-512:09878] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f60b18a4f26]
[fv-az532-512:09878] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f60b18b6d9c]
[fv-az532-512:09878] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f60b18b6e07]
[fv-az532-512:09878] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f60b18b70bb]
[fv-az532-512:09878] [ 8] plumed_master(+0x12ebf)[0x55ebdbaedebf]
[fv-az532-512:09878] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f60b1429d90]
[fv-az532-512:09878] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f60b1429e40]
[fv-az532-512:09878] [11] plumed_master(+0x13155)[0x55ebdbaee155]
[fv-az532-512:09878] *** End of error message ***
</pre>
{% endraw %}

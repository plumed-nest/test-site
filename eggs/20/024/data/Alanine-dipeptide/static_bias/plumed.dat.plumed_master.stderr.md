**Project ID:** [plumID:20.024]({{ '/' | absolute_url }}eggs/20/024/)  
Stderr for source:  Alanine-dipeptide/static_bias/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../../GAMBES.aJG3Fd.cpp:23:10: fatal error: core/Atoms.h: No such file or directory
23 | #include "core/Atoms.h"
|          ^~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../../GAMBES.cpp

[fv-az532-512:09937] *** Process received signal ***
[fv-az532-512:09937] Signal: Aborted (6)
[fv-az532-512:09937] Signal code:  (-6)
[fv-az532-512:09937] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ff629842520]
[fv-az532-512:09937] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ff6298969fc]
[fv-az532-512:09937] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ff629842476]
[fv-az532-512:09937] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ff6298287f3]
[fv-az532-512:09937] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7ff629ca4f26]
[fv-az532-512:09937] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7ff629cb6d9c]
[fv-az532-512:09937] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7ff629cb6e07]
[fv-az532-512:09937] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ff629cb70bb]
[fv-az532-512:09937] [ 8] plumed_master(+0x12ebf)[0x55732c1c8ebf]
[fv-az532-512:09937] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ff629829d90]
[fv-az532-512:09937] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ff629829e40]
[fv-az532-512:09937] [11] plumed_master(+0x13155)[0x55732c1c9155]
[fv-az532-512:09937] *** End of error message ***
</pre>
{% endraw %}

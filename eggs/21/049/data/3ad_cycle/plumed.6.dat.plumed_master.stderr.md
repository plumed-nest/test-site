**Project ID:** [plumID:21.049]({{ '/' | absolute_url }}eggs/21/049/)  
Stderr for source:  3ad_cycle/plumed.6.dat   
Download: [zipped raw stdout](plumed.6.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.6.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../PathCV.0Akmxy.cpp:25:10: fatal error: core/Atoms.h: No such file or directory
25 | #include "core/Atoms.h"
|          ^~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../PathCV.cpp

[fv-az532-512:08567] *** Process received signal ***
[fv-az532-512:08567] Signal: Aborted (6)
[fv-az532-512:08567] Signal code:  (-6)
[fv-az532-512:08567] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb92ca42520]
[fv-az532-512:08567] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb92ca969fc]
[fv-az532-512:08567] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb92ca42476]
[fv-az532-512:08567] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb92ca287f3]
[fv-az532-512:08567] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fb92cea4f26]
[fv-az532-512:08567] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fb92ceb6d9c]
[fv-az532-512:08567] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fb92ceb6e07]
[fv-az532-512:08567] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb92ceb70bb]
[fv-az532-512:08567] [ 8] plumed_master(+0x12ebf)[0x564f2e999ebf]
[fv-az532-512:08567] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb92ca29d90]
[fv-az532-512:08567] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb92ca29e40]
[fv-az532-512:08567] [11] plumed_master(+0x13155)[0x564f2e99a155]
[fv-az532-512:08567] *** End of error message ***
</pre>
{% endraw %}

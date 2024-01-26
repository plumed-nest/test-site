**Project ID:** [plumID:21.049]({{ '/' | absolute_url }}eggs/21/049/)  
Stderr for source:  2ad_inter/plumed.3.dat   
Download: [zipped raw stdout](plumed.3.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.3.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
../PathCV.LJxZe0.cpp:25:10: fatal error: core/Atoms.h: No such file or directory
25 | #include "core/Atoms.h"
|          ^~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../PathCV.cpp

[fv-az532-512:08166] *** Process received signal ***
[fv-az532-512:08166] Signal: Aborted (6)
[fv-az532-512:08166] Signal code:  (-6)
[fv-az532-512:08166] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2fb9042520]
[fv-az532-512:08166] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2fb90969fc]
[fv-az532-512:08166] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2fb9042476]
[fv-az532-512:08166] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2fb90287f3]
[fv-az532-512:08166] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f2fb94a4f26]
[fv-az532-512:08166] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f2fb94b6d9c]
[fv-az532-512:08166] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f2fb94b6e07]
[fv-az532-512:08166] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f2fb94b70bb]
[fv-az532-512:08166] [ 8] plumed_master(+0x12ebf)[0x5616ec17bebf]
[fv-az532-512:08166] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2fb9029d90]
[fv-az532-512:08166] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2fb9029e40]
[fv-az532-512:08166] [11] plumed_master(+0x13155)[0x5616ec17c155]
[fv-az532-512:08166] *** End of error message ***
</pre>
{% endraw %}

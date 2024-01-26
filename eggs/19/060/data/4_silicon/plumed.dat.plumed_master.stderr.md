**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
Stderr for source:  4_silicon/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../0_code/NeuralNetworkVes.9HWYbQ.cpp:29:10: fatal error: core/Atoms.h: No such file or directory
29 | #include "core/Atoms.h"
|          ^~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../0_code/NeuralNetworkVes.cpp

[fv-az979-741:08594] *** Process received signal ***
[fv-az979-741:08594] Signal: Aborted (6)
[fv-az979-741:08594] Signal code:  (-6)
[fv-az979-741:08594] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7febd4e42520]
[fv-az979-741:08594] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7febd4e969fc]
[fv-az979-741:08594] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7febd4e42476]
[fv-az979-741:08594] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7febd4e287f3]
[fv-az979-741:08594] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7febd52a4f26]
[fv-az979-741:08594] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7febd52b6d9c]
[fv-az979-741:08594] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7febd52b6e07]
[fv-az979-741:08594] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7febd52b70bb]
[fv-az979-741:08594] [ 8] plumed_master(+0x12ebf)[0x56144f864ebf]
[fv-az979-741:08594] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7febd4e29d90]
[fv-az979-741:08594] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7febd4e29e40]
[fv-az979-741:08594] [11] plumed_master(+0x13155)[0x56144f865155]
[fv-az979-741:08594] *** End of error message ***
</pre>
{% endraw %}

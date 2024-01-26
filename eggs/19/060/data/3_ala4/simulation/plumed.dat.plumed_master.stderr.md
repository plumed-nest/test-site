**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
Stderr for source:  3_ala4/simulation/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../0_code/NeuralNetworkVes.si0k3W.cpp:29:10: fatal error: core/Atoms.h: No such file or directory
29 | #include "core/Atoms.h"
|          ^~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../../0_code/NeuralNetworkVes.cpp

[fv-az979-741:08534] *** Process received signal ***
[fv-az979-741:08534] Signal: Aborted (6)
[fv-az979-741:08534] Signal code:  (-6)
[fv-az979-741:08534] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa09a442520]
[fv-az979-741:08534] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa09a4969fc]
[fv-az979-741:08534] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa09a442476]
[fv-az979-741:08534] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa09a4287f3]
[fv-az979-741:08534] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fa09a8a4f26]
[fv-az979-741:08534] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fa09a8b6d9c]
[fv-az979-741:08534] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fa09a8b6e07]
[fv-az979-741:08534] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa09a8b70bb]
[fv-az979-741:08534] [ 8] plumed_master(+0x12ebf)[0x55f6300b9ebf]
[fv-az979-741:08534] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa09a429d90]
[fv-az979-741:08534] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa09a429e40]
[fv-az979-741:08534] [11] plumed_master(+0x13155)[0x55f6300ba155]
[fv-az979-741:08534] *** End of error message ***
</pre>
{% endraw %}

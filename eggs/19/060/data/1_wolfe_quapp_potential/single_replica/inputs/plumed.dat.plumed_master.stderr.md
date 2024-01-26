**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
Stderr for source:  1_wolfe_quapp_potential/single_replica/inputs/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../../0_code/NeuralNetworkVes.aQwssT.cpp:29:10: fatal error: core/Atoms.h: No such file or directory
29 | #include "core/Atoms.h"
|          ^~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1254) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_VERSION="2.10.0-dev" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../../../0_code/NeuralNetworkVes.cpp

[fv-az979-741:08418] *** Process received signal ***
[fv-az979-741:08418] Signal: Aborted (6)
[fv-az979-741:08418] Signal code:  (-6)
[fv-az979-741:08418] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7faecf442520]
[fv-az979-741:08418] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7faecf4969fc]
[fv-az979-741:08418] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7faecf442476]
[fv-az979-741:08418] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7faecf4287f3]
[fv-az979-741:08418] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7faecf8a4f26]
[fv-az979-741:08418] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7faecf8b6d9c]
[fv-az979-741:08418] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7faecf8b6e07]
[fv-az979-741:08418] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7faecf8b70bb]
[fv-az979-741:08418] [ 8] plumed_master(+0x12ebf)[0x55f35f2b5ebf]
[fv-az979-741:08418] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7faecf429d90]
[fv-az979-741:08418] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7faecf429e40]
[fv-az979-741:08418] [11] plumed_master(+0x13155)[0x55f35f2b6155]
[fv-az979-741:08418] *** End of error message ***
</pre>
{% endraw %}

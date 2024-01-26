**Project ID:** [plumID:20.003]({{ '/' | absolute_url }}eggs/20/003/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
TD_TS-target-plumed2.6.cpp:23:10: fatal error: TargetDistribution.h: No such file or directory
23 | #include "TargetDistribution.h"
|          ^~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1070) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed" env PLUMED_VERSION="2.9.0" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed"/scripts/mklib.sh TD_TS-target-plumed2.6.cpp

[fv-az1200-577:09343] *** Process received signal ***
[fv-az1200-577:09343] Signal: Aborted (6)
[fv-az1200-577:09343] Signal code:  (-6)
[fv-az1200-577:09343] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f93cb642520]
[fv-az1200-577:09343] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f93cb6969fc]
[fv-az1200-577:09343] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f93cb642476]
[fv-az1200-577:09343] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f93cb6287f3]
[fv-az1200-577:09343] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f93cbaa4f26]
[fv-az1200-577:09343] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f93cbab6d9c]
[fv-az1200-577:09343] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f93cbab6e07]
[fv-az1200-577:09343] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f93cbab70bb]
[fv-az1200-577:09343] [ 8] plumed(+0x12f48)[0x55c662989f48]
[fv-az1200-577:09343] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f93cb629d90]
[fv-az1200-577:09343] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f93cb629e40]
[fv-az1200-577:09343] [11] plumed(+0x131e5)[0x55c66298a1e5]
[fv-az1200-577:09343] *** End of error message ***
</pre>
{% endraw %}

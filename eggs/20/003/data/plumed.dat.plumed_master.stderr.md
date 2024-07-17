**Project ID:** [plumID:20.003]({{ '/' | absolute_url }}eggs/20/003/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
TD_TS-target-plumed2.6.ltc7nt.cpp:23:10: fatal error: TargetDistribution.h: No such file or directory
23 | #include "TargetDistribution.h"
|          ^~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1292) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./TD_TS-target-plumed2.6.2.10.0-dev.so TD_TS-target-plumed2.6.cpp

[fv-az774-16:74366] *** Process received signal ***
[fv-az774-16:74366] Signal: Aborted (6)
[fv-az774-16:74366] Signal code:  (-6)
[fv-az774-16:74366] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1476042520]
[fv-az774-16:74366] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f14760969fc]
[fv-az774-16:74366] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1476042476]
[fv-az774-16:74366] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f14760287f3]
[fv-az774-16:74366] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f14764a2b9e]
[fv-az774-16:74366] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f14764ae20c]
[fv-az774-16:74366] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f14764ae277]
[fv-az774-16:74366] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f14764ae52b]
[fv-az774-16:74366] [ 8] plumed_master(+0x14274)[0x55dc1a2b9274]
[fv-az774-16:74366] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1476029d90]
[fv-az774-16:74366] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1476029e40]
[fv-az774-16:74366] [11] plumed_master(+0x14ed5)[0x55dc1a2b9ed5]
[fv-az774-16:74366] *** End of error message ***
</pre>
{% endraw %}

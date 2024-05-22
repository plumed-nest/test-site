**Project ID:** [plumID:20.003]({{ '/' | absolute_url }}eggs/20/003/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
TD_TS-target-plumed2.6.raDw95.cpp:23:10: fatal error: TargetDistribution.h: No such file or directory
23 | #include "TargetDistribution.h"
|          ^~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1282) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./TD_TS-target-plumed2.6.2.10.0-dev.so TD_TS-target-plumed2.6.cpp

[fv-az1106-239:43933] *** Process received signal ***
[fv-az1106-239:43933] Signal: Aborted (6)
[fv-az1106-239:43933] Signal code:  (-6)
[fv-az1106-239:43933] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f93f6442520]
[fv-az1106-239:43933] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f93f64969fc]
[fv-az1106-239:43933] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f93f6442476]
[fv-az1106-239:43933] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f93f64287f3]
[fv-az1106-239:43933] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f93f68a2b9e]
[fv-az1106-239:43933] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f93f68ae20c]
[fv-az1106-239:43933] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f93f68ae277]
[fv-az1106-239:43933] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f93f68ae52b]
[fv-az1106-239:43933] [ 8] plumed_master(+0x14274)[0x5592017f2274]
[fv-az1106-239:43933] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f93f6429d90]
[fv-az1106-239:43933] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f93f6429e40]
[fv-az1106-239:43933] [11] plumed_master(+0x14ed5)[0x5592017f2ed5]
[fv-az1106-239:43933] *** End of error message ***
</pre>
{% endraw %}

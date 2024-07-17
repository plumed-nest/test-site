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
(core/PlumedMain.cpp:1071) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.9.1' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh TD_TS-target-plumed2.6.cpp

[fv-az774-16:74352] *** Process received signal ***
[fv-az774-16:74352] Signal: Aborted (6)
[fv-az774-16:74352] Signal code:  (-6)
[fv-az774-16:74352] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3044242520]
[fv-az774-16:74352] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f30442969fc]
[fv-az774-16:74352] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3044242476]
[fv-az774-16:74352] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f30442287f3]
[fv-az774-16:74352] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f30446a2b9e]
[fv-az774-16:74352] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f30446ae20c]
[fv-az774-16:74352] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f30446ae277]
[fv-az774-16:74352] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f30446ae52b]
[fv-az774-16:74352] [ 8] plumed(+0x12f48)[0x55a781bdcf48]
[fv-az774-16:74352] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3044229d90]
[fv-az774-16:74352] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3044229e40]
[fv-az774-16:74352] [11] plumed(+0x131e5)[0x55a781bdd1e5]
[fv-az774-16:74352] *** End of error message ***
</pre>
{% endraw %}

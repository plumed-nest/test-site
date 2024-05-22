**Project ID:** [plumID:22.014]({{ '/' | absolute_url }}eggs/22/014/)  
Stderr for source:  plumed-order-parameters.dat   
Download: [zipped raw stdout](plumed-order-parameters.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-order-parameters.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
PairEntropies.CPO4Pw.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1282) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./PairEntropies.2.10.0-dev.so PairEntropies.cpp

[fv-az1109-238:40076] *** Process received signal ***
[fv-az1109-238:40076] Signal: Aborted (6)
[fv-az1109-238:40076] Signal code:  (-6)
[fv-az1109-238:40076] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc6ada42520]
[fv-az1109-238:40076] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc6ada969fc]
[fv-az1109-238:40076] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc6ada42476]
[fv-az1109-238:40076] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc6ada287f3]
[fv-az1109-238:40076] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc6adea2b9e]
[fv-az1109-238:40076] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc6adeae20c]
[fv-az1109-238:40076] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc6adeae277]
[fv-az1109-238:40076] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc6adeae52b]
[fv-az1109-238:40076] [ 8] plumed_master(+0x14274)[0x556df72d8274]
[fv-az1109-238:40076] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc6ada29d90]
[fv-az1109-238:40076] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc6ada29e40]
[fv-az1109-238:40076] [11] plumed_master(+0x14ed5)[0x556df72d8ed5]
[fv-az1109-238:40076] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:22.014]({{ '/' | absolute_url }}eggs/22/014/)  
Stderr for source:  plumed-order-parameters.dat   
Download: [zipped raw stdout](plumed-order-parameters.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-order-parameters.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
PairEntropies.Czu5Mp.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1292) void PLMD::PlumedMain::load(const string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.10.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./PairEntropies.2.10.0-dev.so PairEntropies.cpp

[fv-az659-178:70326] *** Process received signal ***
[fv-az659-178:70326] Signal: Aborted (6)
[fv-az659-178:70326] Signal code:  (-6)
[fv-az659-178:70326] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdcc9442520]
[fv-az659-178:70326] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdcc94969fc]
[fv-az659-178:70326] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdcc9442476]
[fv-az659-178:70326] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdcc94287f3]
[fv-az659-178:70326] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fdcc98a2b9e]
[fv-az659-178:70326] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fdcc98ae20c]
[fv-az659-178:70326] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fdcc98ae277]
[fv-az659-178:70326] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdcc98ae52b]
[fv-az659-178:70326] [ 8] plumed_master(+0x14274)[0x559c6ad21274]
[fv-az659-178:70326] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdcc9429d90]
[fv-az659-178:70326] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdcc9429e40]
[fv-az659-178:70326] [11] plumed_master(+0x14ed5)[0x559c6ad21ed5]
[fv-az659-178:70326] *** End of error message ***
</pre>
{% endraw %}

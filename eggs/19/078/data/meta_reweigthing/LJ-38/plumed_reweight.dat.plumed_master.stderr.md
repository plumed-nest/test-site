**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action COLLECT with label cc_ns : missing TYPE keyword.  TYPE should specify whether data is to be stored as a vector or a matrix
[fv-az695-456:75839] *** Process received signal ***
[fv-az695-456:75839] Signal: Aborted (6)
[fv-az695-456:75839] Signal code:  (-6)
[fv-az695-456:75839] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc839e42520]
[fv-az695-456:75839] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc839e969fc]
[fv-az695-456:75839] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc839e42476]
[fv-az695-456:75839] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc839e287f3]
[fv-az695-456:75839] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc83a2a2b9e]
[fv-az695-456:75839] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc83a2ae20c]
[fv-az695-456:75839] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc83a2ae277]
[fv-az695-456:75839] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc83a2ae52b]
[fv-az695-456:75839] [ 8] plumed_master(+0x14274)[0x56540e7ce274]
[fv-az695-456:75839] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc839e29d90]
[fv-az695-456:75839] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc839e29e40]
[fv-az695-456:75839] [11] plumed_master(+0x14ed5)[0x56540e7ceed5]
[fv-az695-456:75839] *** End of error message ***
</pre>
{% endraw %}

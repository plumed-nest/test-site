**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action COLLECT with label cc_ns : missing TYPE keyword.  TYPE should specify whether data is to be stored as a vector or a matrix
[fv-az1113-981:45340] *** Process received signal ***
[fv-az1113-981:45340] Signal: Aborted (6)
[fv-az1113-981:45340] Signal code:  (-6)
[fv-az1113-981:45340] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdadd842520]
[fv-az1113-981:45340] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdadd8969fc]
[fv-az1113-981:45340] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdadd842476]
[fv-az1113-981:45340] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdadd8287f3]
[fv-az1113-981:45340] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fdaddca2b9e]
[fv-az1113-981:45340] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fdaddcae20c]
[fv-az1113-981:45340] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fdaddcae277]
[fv-az1113-981:45340] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdaddcae52b]
[fv-az1113-981:45340] [ 8] plumed_master(+0x14274)[0x5571bbd9e274]
[fv-az1113-981:45340] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdadd829d90]
[fv-az1113-981:45340] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdadd829e40]
[fv-az1113-981:45340] [11] plumed_master(+0x14ed5)[0x5571bbd9eed5]
[fv-az1113-981:45340] *** End of error message ***
</pre>
{% endraw %}

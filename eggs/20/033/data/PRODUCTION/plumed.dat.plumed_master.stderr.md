**Project ID:** [plumID:20.033]({{ '/' | absolute_url }}eggs/20/033/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action WHOLEMOLECULES with label @5 : cannot understand the following words from the input line : REF0=16.995,21.964,24.520, REF1=26.253,18.440,24.5030, REF2=24.616,28.069,24.203
[fv-az1106-239:43673] *** Process received signal ***
[fv-az1106-239:43673] Signal: Aborted (6)
[fv-az1106-239:43673] Signal code:  (-6)
[fv-az1106-239:43673] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd11b242520]
[fv-az1106-239:43673] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd11b2969fc]
[fv-az1106-239:43673] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd11b242476]
[fv-az1106-239:43673] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd11b2287f3]
[fv-az1106-239:43673] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd11b6a2b9e]
[fv-az1106-239:43673] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd11b6ae20c]
[fv-az1106-239:43673] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd11b6ae277]
[fv-az1106-239:43673] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd11b6ae52b]
[fv-az1106-239:43673] [ 8] plumed_master(+0x14274)[0x556c58e9a274]
[fv-az1106-239:43673] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd11b229d90]
[fv-az1106-239:43673] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd11b229e40]
[fv-az1106-239:43673] [11] plumed_master(+0x14ed5)[0x556c58e9aed5]
[fv-az1106-239:43673] *** End of error message ***
</pre>
{% endraw %}

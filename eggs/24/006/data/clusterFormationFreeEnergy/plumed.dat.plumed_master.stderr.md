**Project ID:** [plumID:24.006]({{ '/' | absolute_url }}eggs/24/006/)  
Stderr for source:  clusterFormationFreeEnergy/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action CLUSTER_PROPERTIES with label @s22 : keyword ARG is compulsory for this action
[fv-az1435-553:39064] *** Process received signal ***
[fv-az1435-553:39064] Signal: Aborted (6)
[fv-az1435-553:39064] Signal code:  (-6)
[fv-az1435-553:39064] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3891c42520]
[fv-az1435-553:39064] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3891c969fc]
[fv-az1435-553:39064] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3891c42476]
[fv-az1435-553:39064] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3891c287f3]
[fv-az1435-553:39064] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f38920a2b9e]
[fv-az1435-553:39064] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f38920ae20c]
[fv-az1435-553:39064] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f38920ae277]
[fv-az1435-553:39064] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f38920ae52b]
[fv-az1435-553:39064] [ 8] plumed_master(+0x14274)[0x556ce16ca274]
[fv-az1435-553:39064] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3891c29d90]
[fv-az1435-553:39064] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3891c29e40]
[fv-az1435-553:39064] [11] plumed_master(+0x14ed5)[0x556ce16caed5]
[fv-az1435-553:39064] *** End of error message ***
</pre>
{% endraw %}

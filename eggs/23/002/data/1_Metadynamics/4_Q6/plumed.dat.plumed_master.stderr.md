**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  1_Metadynamics/4_Q6/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action LOCAL_AVERAGE with label @s28 : cannot understand the following words from the input line : LOWMEM
[fv-az1435-553:40065] *** Process received signal ***
[fv-az1435-553:40065] Signal: Aborted (6)
[fv-az1435-553:40065] Signal code:  (-6)
[fv-az1435-553:40065] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5b6c842520]
[fv-az1435-553:40065] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5b6c8969fc]
[fv-az1435-553:40065] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5b6c842476]
[fv-az1435-553:40065] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5b6c8287f3]
[fv-az1435-553:40065] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f5b6cca2b9e]
[fv-az1435-553:40065] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f5b6ccae20c]
[fv-az1435-553:40065] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f5b6ccae277]
[fv-az1435-553:40065] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5b6ccae52b]
[fv-az1435-553:40065] [ 8] plumed_master(+0x14274)[0x559346890274]
[fv-az1435-553:40065] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5b6c829d90]
[fv-az1435-553:40065] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5b6c829e40]
[fv-az1435-553:40065] [11] plumed_master(+0x14ed5)[0x559346890ed5]
[fv-az1435-553:40065] *** End of error message ***
</pre>
{% endraw %}

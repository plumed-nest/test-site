**Project ID:** [plumID:22.028]({{ '/' | absolute_url }}eggs/22/028/)  
Stderr for source:  plumed_pucker.dat   
Download: [zipped raw stdout](plumed_pucker.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_pucker.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label puck1 : could not find file named COLVAR_theta.0
[fv-az1435-553:40386] *** Process received signal ***
[fv-az1435-553:40386] Signal: Aborted (6)
[fv-az1435-553:40386] Signal code:  (-6)
[fv-az1435-553:40386] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6e9b042520]
[fv-az1435-553:40386] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6e9b0969fc]
[fv-az1435-553:40386] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6e9b042476]
[fv-az1435-553:40386] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6e9b0287f3]
[fv-az1435-553:40386] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f6e9b4a2b9e]
[fv-az1435-553:40386] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f6e9b4ae20c]
[fv-az1435-553:40386] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f6e9b4ae277]
[fv-az1435-553:40386] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6e9b4ae52b]
[fv-az1435-553:40386] [ 8] plumed_master(+0x14274)[0x55dc57190274]
[fv-az1435-553:40386] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6e9b029d90]
[fv-az1435-553:40386] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6e9b029e40]
[fv-az1435-553:40386] [11] plumed_master(+0x14ed5)[0x55dc57190ed5]
[fv-az1435-553:40386] *** End of error message ***
</pre>
{% endraw %}

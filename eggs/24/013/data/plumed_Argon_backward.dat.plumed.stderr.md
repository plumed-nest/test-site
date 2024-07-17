**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_Argon_backward.dat   
Download: [zipped raw stdout](plumed_Argon_backward.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_backward.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action COORDINATIONNUMBER with label coord : keyword MORE_THAN could not be read correctly
[fv-az975-63:69532] *** Process received signal ***
[fv-az975-63:69532] Signal: Aborted (6)
[fv-az975-63:69532] Signal code:  (-6)
[fv-az975-63:69532] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5747042520]
[fv-az975-63:69532] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f57470969fc]
[fv-az975-63:69532] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5747042476]
[fv-az975-63:69532] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f57470287f3]
[fv-az975-63:69532] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f57474a2b9e]
[fv-az975-63:69532] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f57474ae20c]
[fv-az975-63:69532] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f57474ae277]
[fv-az975-63:69532] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f57474ae52b]
[fv-az975-63:69532] [ 8] plumed(+0x12f48)[0x55a3b30c9f48]
[fv-az975-63:69532] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5747029d90]
[fv-az975-63:69532] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5747029e40]
[fv-az975-63:69532] [11] plumed(+0x131e5)[0x55a3b30ca1e5]
[fv-az975-63:69532] *** End of error message ***
</pre>
{% endraw %}

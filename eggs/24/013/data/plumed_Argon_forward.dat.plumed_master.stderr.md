**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_Argon_forward.dat   
Download: [zipped raw stdout](plumed_Argon_forward.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_forward.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action COORDINATIONNUMBER with label @s11 : keyword MORE_THAN could not be read correctly
[fv-az975-63:69572] *** Process received signal ***
[fv-az975-63:69572] Signal: Aborted (6)
[fv-az975-63:69572] Signal code:  (-6)
[fv-az975-63:69572] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f228d042520]
[fv-az975-63:69572] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f228d0969fc]
[fv-az975-63:69572] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f228d042476]
[fv-az975-63:69572] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f228d0287f3]
[fv-az975-63:69572] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f228d4a2b9e]
[fv-az975-63:69572] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f228d4ae20c]
[fv-az975-63:69572] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f228d4ae277]
[fv-az975-63:69572] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f228d4ae52b]
[fv-az975-63:69572] [ 8] plumed_master(+0x14274)[0x560c44404274]
[fv-az975-63:69572] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f228d029d90]
[fv-az975-63:69572] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f228d029e40]
[fv-az975-63:69572] [11] plumed_master(+0x14ed5)[0x560c44404ed5]
[fv-az975-63:69572] *** End of error message ***
</pre>
{% endraw %}

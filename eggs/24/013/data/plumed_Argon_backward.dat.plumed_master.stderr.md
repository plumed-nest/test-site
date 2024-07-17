**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_Argon_backward.dat   
Download: [zipped raw stdout](plumed_Argon_backward.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_backward.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action COORDINATIONNUMBER with label @s11 : keyword MORE_THAN could not be read correctly
[fv-az975-63:69540] *** Process received signal ***
[fv-az975-63:69540] Signal: Aborted (6)
[fv-az975-63:69540] Signal code:  (-6)
[fv-az975-63:69540] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdaf7c42520]
[fv-az975-63:69540] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdaf7c969fc]
[fv-az975-63:69540] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdaf7c42476]
[fv-az975-63:69540] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdaf7c287f3]
[fv-az975-63:69540] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fdaf80a2b9e]
[fv-az975-63:69540] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fdaf80ae20c]
[fv-az975-63:69540] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fdaf80ae277]
[fv-az975-63:69540] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdaf80ae52b]
[fv-az975-63:69540] [ 8] plumed_master(+0x14274)[0x55bdc872d274]
[fv-az975-63:69540] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdaf7c29d90]
[fv-az975-63:69540] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdaf7c29e40]
[fv-az975-63:69540] [11] plumed_master(+0x14ed5)[0x55bdc872ded5]
[fv-az975-63:69540] *** End of error message ***
</pre>
{% endraw %}

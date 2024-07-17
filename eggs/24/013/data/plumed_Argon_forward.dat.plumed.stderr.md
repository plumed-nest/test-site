**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_Argon_forward.dat   
Download: [zipped raw stdout](plumed_Argon_forward.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_forward.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action COORDINATIONNUMBER with label coord : keyword MORE_THAN could not be read correctly
[fv-az975-63:69564] *** Process received signal ***
[fv-az975-63:69564] Signal: Aborted (6)
[fv-az975-63:69564] Signal code:  (-6)
[fv-az975-63:69564] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fed75442520]
[fv-az975-63:69564] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fed754969fc]
[fv-az975-63:69564] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fed75442476]
[fv-az975-63:69564] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fed754287f3]
[fv-az975-63:69564] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fed758a2b9e]
[fv-az975-63:69564] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fed758ae20c]
[fv-az975-63:69564] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fed758ae277]
[fv-az975-63:69564] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fed758ae52b]
[fv-az975-63:69564] [ 8] plumed(+0x12f48)[0x5618771adf48]
[fv-az975-63:69564] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fed75429d90]
[fv-az975-63:69564] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fed75429e40]
[fv-az975-63:69564] [11] plumed(+0x131e5)[0x5618771ae1e5]
[fv-az975-63:69564] *** End of error message ***
</pre>
{% endraw %}

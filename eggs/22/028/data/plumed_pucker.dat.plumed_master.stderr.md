**Project ID:** [plumID:22.028]({{ '/' | absolute_url }}eggs/22/028/)  
Stderr for source:  plumed_pucker.dat   
Download: [zipped raw stdout](plumed_pucker.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_pucker.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label puck1 : could not find file named COLVAR_theta.0
[fv-az774-16:70771] *** Process received signal ***
[fv-az774-16:70771] Signal: Aborted (6)
[fv-az774-16:70771] Signal code:  (-6)
[fv-az774-16:70771] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f506be42520]
[fv-az774-16:70771] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f506be969fc]
[fv-az774-16:70771] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f506be42476]
[fv-az774-16:70771] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f506be287f3]
[fv-az774-16:70771] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f506c2a2b9e]
[fv-az774-16:70771] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f506c2ae20c]
[fv-az774-16:70771] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f506c2ae277]
[fv-az774-16:70771] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f506c2ae52b]
[fv-az774-16:70771] [ 8] plumed_master(+0x14274)[0x562795af0274]
[fv-az774-16:70771] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f506be29d90]
[fv-az774-16:70771] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f506be29e40]
[fv-az774-16:70771] [11] plumed_master(+0x14ed5)[0x562795af0ed5]
[fv-az774-16:70771] *** End of error message ***
</pre>
{% endraw %}
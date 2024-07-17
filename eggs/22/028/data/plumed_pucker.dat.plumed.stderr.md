**Project ID:** [plumID:22.028]({{ '/' | absolute_url }}eggs/22/028/)  
Stderr for source:  plumed_pucker.dat   
Download: [zipped raw stdout](plumed_pucker.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_pucker.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label puck1 : could not find file named COLVAR_theta.0
[fv-az774-16:70763] *** Process received signal ***
[fv-az774-16:70763] Signal: Aborted (6)
[fv-az774-16:70763] Signal code:  (-6)
[fv-az774-16:70763] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4584042520]
[fv-az774-16:70763] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f45840969fc]
[fv-az774-16:70763] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4584042476]
[fv-az774-16:70763] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f45840287f3]
[fv-az774-16:70763] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f45844a2b9e]
[fv-az774-16:70763] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f45844ae20c]
[fv-az774-16:70763] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f45844ae277]
[fv-az774-16:70763] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f45844ae52b]
[fv-az774-16:70763] [ 8] plumed(+0x12f48)[0x558c487aef48]
[fv-az774-16:70763] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4584029d90]
[fv-az774-16:70763] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4584029e40]
[fv-az774-16:70763] [11] plumed(+0x131e5)[0x558c487af1e5]
[fv-az774-16:70763] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:22.028]({{ '/' | absolute_url }}eggs/22/028/)  
Stderr for source:  plumed_pucker.dat   
Download: [zipped raw stdout](plumed_pucker.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_pucker.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label puck1 : could not find file named COLVAR_theta.0
[fv-az529-343:05595] *** Process received signal ***
[fv-az529-343:05595] Signal: Aborted (6)
[fv-az529-343:05595] Signal code:  (-6)
[fv-az529-343:05595] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fed82a42520]
[fv-az529-343:05595] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fed82a969fc]
[fv-az529-343:05595] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fed82a42476]
[fv-az529-343:05595] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fed82a287f3]
[fv-az529-343:05595] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fed82ea4f26]
[fv-az529-343:05595] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fed82eb6d9c]
[fv-az529-343:05595] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fed82eb6e07]
[fv-az529-343:05595] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fed82eb70bb]
[fv-az529-343:05595] [ 8] plumed(+0x12f48)[0x55dc117c9f48]
[fv-az529-343:05595] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fed82a29d90]
[fv-az529-343:05595] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fed82a29e40]
[fv-az529-343:05595] [11] plumed(+0x131e5)[0x55dc117ca1e5]
[fv-az529-343:05595] *** End of error message ***
</pre>
{% endraw %}

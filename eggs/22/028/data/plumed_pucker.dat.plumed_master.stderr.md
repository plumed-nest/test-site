**Project ID:** [plumID:22.028]({{ '/' | absolute_url }}eggs/22/028/)  
Stderr for source:  plumed_pucker.dat   
Download: [zipped raw stdout](plumed_pucker.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_pucker.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label puck1 : could not find file named COLVAR_theta.0
[fv-az529-343:05603] *** Process received signal ***
[fv-az529-343:05603] Signal: Aborted (6)
[fv-az529-343:05603] Signal code:  (-6)
[fv-az529-343:05603] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdff1042520]
[fv-az529-343:05603] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdff10969fc]
[fv-az529-343:05603] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdff1042476]
[fv-az529-343:05603] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdff10287f3]
[fv-az529-343:05603] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fdff14a4f26]
[fv-az529-343:05603] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fdff14b6d9c]
[fv-az529-343:05603] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fdff14b6e07]
[fv-az529-343:05603] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdff14b70bb]
[fv-az529-343:05603] [ 8] plumed_master(+0x12ebf)[0x55d8559e5ebf]
[fv-az529-343:05603] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdff1029d90]
[fv-az529-343:05603] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdff1029e40]
[fv-az529-343:05603] [11] plumed_master(+0x13155)[0x55d8559e6155]
[fv-az529-343:05603] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:19.032]({{ '/' | absolute_url }}eggs/19/032/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : restart file HILLS not found
[fv-az1148-6:10155] *** Process received signal ***
[fv-az1148-6:10155] Signal: Aborted (6)
[fv-az1148-6:10155] Signal code:  (-6)
[fv-az1148-6:10155] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0a48842520]
[fv-az1148-6:10155] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0a488969fc]
[fv-az1148-6:10155] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0a48842476]
[fv-az1148-6:10155] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0a488287f3]
[fv-az1148-6:10155] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f0a48ca4f26]
[fv-az1148-6:10155] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f0a48cb6d9c]
[fv-az1148-6:10155] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f0a48cb6e07]
[fv-az1148-6:10155] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f0a48cb70bb]
[fv-az1148-6:10155] [ 8] plumed_master(+0x12ebf)[0x56489a138ebf]
[fv-az1148-6:10155] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0a48829d90]
[fv-az1148-6:10155] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0a48829e40]
[fv-az1148-6:10155] [11] plumed_master(+0x13155)[0x56489a139155]
[fv-az1148-6:10155] *** End of error message ***
</pre>
{% endraw %}

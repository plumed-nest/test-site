**Project ID:** [plumID:20.002]({{ '/' | absolute_url }}eggs/20/002/)  
Stderr for source:  plumed-MetaD.dat   
Download: [zipped raw stdout](plumed-MetaD.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-MetaD.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : restart file HILLS not found
[fv-az736-136:09783] *** Process received signal ***
[fv-az736-136:09783] Signal: Aborted (6)
[fv-az736-136:09783] Signal code:  (-6)
[fv-az736-136:09783] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc2fee42520]
[fv-az736-136:09783] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc2fee969fc]
[fv-az736-136:09783] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc2fee42476]
[fv-az736-136:09783] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc2fee287f3]
[fv-az736-136:09783] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fc2ff2a4f26]
[fv-az736-136:09783] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fc2ff2b6d9c]
[fv-az736-136:09783] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fc2ff2b6e07]
[fv-az736-136:09783] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc2ff2b70bb]
[fv-az736-136:09783] [ 8] plumed_master(+0x12ebf)[0x55997d9fcebf]
[fv-az736-136:09783] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc2fee29d90]
[fv-az736-136:09783] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc2fee29e40]
[fv-az736-136:09783] [11] plumed_master(+0x13155)[0x55997d9fd155]
[fv-az736-136:09783] *** End of error message ***
</pre>
{% endraw %}

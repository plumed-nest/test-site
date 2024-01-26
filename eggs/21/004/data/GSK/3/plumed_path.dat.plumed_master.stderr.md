**Project ID:** [plumID:21.004]({{ '/' | absolute_url }}eggs/21/004/)  
Stderr for source:  GSK/3/plumed_path.dat   
Download: [zipped raw stdout](plumed_path.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_path.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : restart file HILLS not found
[fv-az1542-52:07811] *** Process received signal ***
[fv-az1542-52:07811] Signal: Aborted (6)
[fv-az1542-52:07811] Signal code:  (-6)
[fv-az1542-52:07811] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1c65842520]
[fv-az1542-52:07811] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1c658969fc]
[fv-az1542-52:07811] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1c65842476]
[fv-az1542-52:07811] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1c658287f3]
[fv-az1542-52:07811] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f1c65ca4f26]
[fv-az1542-52:07811] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f1c65cb6d9c]
[fv-az1542-52:07811] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f1c65cb6e07]
[fv-az1542-52:07811] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1c65cb70bb]
[fv-az1542-52:07811] [ 8] plumed_master(+0x12ebf)[0x55c701db6ebf]
[fv-az1542-52:07811] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1c65829d90]
[fv-az1542-52:07811] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1c65829e40]
[fv-az1542-52:07811] [11] plumed_master(+0x13155)[0x55c701db7155]
[fv-az1542-52:07811] *** End of error message ***
</pre>
{% endraw %}

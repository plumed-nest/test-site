**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_mo.dat   
Download: [zipped raw stdout](plumed_mo.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_mo.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label @0 : Number of specified atoms should be 2
[fv-az532-512:09400] *** Process received signal ***
[fv-az532-512:09400] Signal: Aborted (6)
[fv-az532-512:09400] Signal code:  (-6)
[fv-az532-512:09400] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f069a042520]
[fv-az532-512:09400] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f069a0969fc]
[fv-az532-512:09400] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f069a042476]
[fv-az532-512:09400] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f069a0287f3]
[fv-az532-512:09400] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f069a4a4f26]
[fv-az532-512:09400] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f069a4b6d9c]
[fv-az532-512:09400] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f069a4b6e07]
[fv-az532-512:09400] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f069a4b70bb]
[fv-az532-512:09400] [ 8] plumed_master(+0x12ebf)[0x559eef28cebf]
[fv-az532-512:09400] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f069a029d90]
[fv-az532-512:09400] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f069a029e40]
[fv-az532-512:09400] [11] plumed_master(+0x13155)[0x559eef28d155]
[fv-az532-512:09400] *** End of error message ***
</pre>
{% endraw %}

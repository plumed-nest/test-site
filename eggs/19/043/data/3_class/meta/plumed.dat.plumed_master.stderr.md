**Project ID:** [plumID:19.043]({{ '/' | absolute_url }}eggs/19/043/)  
Stderr for source:  3_class/meta/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1542-52:08629] *** Process received signal ***
[fv-az1542-52:08629] Signal: Aborted (6)
[fv-az1542-52:08629] Signal code:  (-6)
[fv-az1542-52:08629] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd769e42520]
[fv-az1542-52:08629] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd769e969fc]
[fv-az1542-52:08629] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd769e42476]
[fv-az1542-52:08629] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd769e287f3]
[fv-az1542-52:08629] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fd76a2a4f26]
[fv-az1542-52:08629] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fd76a2b6d9c]
[fv-az1542-52:08629] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fd76a2b6e07]
[fv-az1542-52:08629] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd76a2b70bb]
[fv-az1542-52:08629] [ 8] plumed_master(+0x12ebf)[0x55ecb2cacebf]
[fv-az1542-52:08629] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd769e29d90]
[fv-az1542-52:08629] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd769e29e40]
[fv-az1542-52:08629] [11] plumed_master(+0x13155)[0x55ecb2cad155]
[fv-az1542-52:08629] *** End of error message ***
</pre>
{% endraw %}

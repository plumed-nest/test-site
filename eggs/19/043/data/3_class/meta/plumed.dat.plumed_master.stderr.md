**Project ID:** [plumID:19.043]({{ '/' | absolute_url }}eggs/19/043/)  
Stderr for source:  3_class/meta/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az841-65:73624] *** Process received signal ***
[fv-az841-65:73624] Signal: Aborted (6)
[fv-az841-65:73624] Signal code:  (-6)
[fv-az841-65:73624] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ff34be42520]
[fv-az841-65:73624] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ff34be969fc]
[fv-az841-65:73624] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ff34be42476]
[fv-az841-65:73624] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ff34be287f3]
[fv-az841-65:73624] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7ff34c2a2b9e]
[fv-az841-65:73624] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7ff34c2ae20c]
[fv-az841-65:73624] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7ff34c2ae277]
[fv-az841-65:73624] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ff34c2ae52b]
[fv-az841-65:73624] [ 8] plumed_master(+0x14274)[0x558c5f1f1274]
[fv-az841-65:73624] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ff34be29d90]
[fv-az841-65:73624] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ff34be29e40]
[fv-az841-65:73624] [11] plumed_master(+0x14ed5)[0x558c5f1f1ed5]
[fv-az841-65:73624] *** End of error message ***
</pre>
{% endraw %}

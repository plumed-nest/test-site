**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
Stderr for source:  ache-pwf/plumed-biased.dat   
Download: [zipped raw stdout](plumed-biased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-biased.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1200-577:09893] *** Process received signal ***
[fv-az1200-577:09893] Signal: Aborted (6)
[fv-az1200-577:09893] Signal code:  (-6)
[fv-az1200-577:09893] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa9b5a42520]
[fv-az1200-577:09893] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa9b5a969fc]
[fv-az1200-577:09893] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa9b5a42476]
[fv-az1200-577:09893] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa9b5a287f3]
[fv-az1200-577:09893] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fa9b5ea4f26]
[fv-az1200-577:09893] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fa9b5eb6d9c]
[fv-az1200-577:09893] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fa9b5eb6e07]
[fv-az1200-577:09893] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa9b5eb70bb]
[fv-az1200-577:09893] [ 8] plumed_master(+0x12ebf)[0x5585cd54febf]
[fv-az1200-577:09893] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa9b5a29d90]
[fv-az1200-577:09893] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa9b5a29e40]
[fv-az1200-577:09893] [11] plumed_master(+0x13155)[0x5585cd550155]
[fv-az1200-577:09893] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:19.061]({{ '/' | absolute_url }}eggs/19/061/)  
Stderr for source:  diffusion_meta.dat   
Download: [zipped raw stdout](diffusion_meta.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](diffusion_meta.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : restart file HILLS not found
[fv-az1493-330:09003] *** Process received signal ***
[fv-az1493-330:09003] Signal: Aborted (6)
[fv-az1493-330:09003] Signal code:  (-6)
[fv-az1493-330:09003] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7f0e042520]
[fv-az1493-330:09003] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7f0e0969fc]
[fv-az1493-330:09003] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7f0e042476]
[fv-az1493-330:09003] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7f0e0287f3]
[fv-az1493-330:09003] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f7f0e4a4f26]
[fv-az1493-330:09003] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f7f0e4b6d9c]
[fv-az1493-330:09003] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f7f0e4b6e07]
[fv-az1493-330:09003] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7f0e4b70bb]
[fv-az1493-330:09003] [ 8] plumed_master(+0x12ebf)[0x55b303b82ebf]
[fv-az1493-330:09003] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7f0e029d90]
[fv-az1493-330:09003] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7f0e029e40]
[fv-az1493-330:09003] [11] plumed_master(+0x13155)[0x55b303b83155]
[fv-az1493-330:09003] *** End of error message ***
</pre>
{% endraw %}

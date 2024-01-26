**Project ID:** [plumID:19.061]({{ '/' | absolute_url }}eggs/19/061/)  
Stderr for source:  ple_meta.dat   
Download: [zipped raw stdout](ple_meta.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](ple_meta.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : restart file HILLS not found
[fv-az1493-330:09034] *** Process received signal ***
[fv-az1493-330:09034] Signal: Aborted (6)
[fv-az1493-330:09034] Signal code:  (-6)
[fv-az1493-330:09034] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9e8b442520]
[fv-az1493-330:09034] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f9e8b4969fc]
[fv-az1493-330:09034] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9e8b442476]
[fv-az1493-330:09034] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f9e8b4287f3]
[fv-az1493-330:09034] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f9e8b8a4f26]
[fv-az1493-330:09034] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f9e8b8b6d9c]
[fv-az1493-330:09034] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f9e8b8b6e07]
[fv-az1493-330:09034] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f9e8b8b70bb]
[fv-az1493-330:09034] [ 8] plumed_master(+0x12ebf)[0x55fe4f881ebf]
[fv-az1493-330:09034] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9e8b429d90]
[fv-az1493-330:09034] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9e8b429e40]
[fv-az1493-330:09034] [11] plumed_master(+0x13155)[0x55fe4f882155]
[fv-az1493-330:09034] *** End of error message ***
</pre>
{% endraw %}

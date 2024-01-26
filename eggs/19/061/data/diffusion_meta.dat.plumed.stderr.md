**Project ID:** [plumID:19.061]({{ '/' | absolute_url }}eggs/19/061/)  
Stderr for source:  diffusion_meta.dat   
Download: [zipped raw stdout](diffusion_meta.dat.plumed.stdout.txt.zip) - [zipped raw stderr](diffusion_meta.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : restart file HILLS not found
[fv-az1493-330:08995] *** Process received signal ***
[fv-az1493-330:08995] Signal: Aborted (6)
[fv-az1493-330:08995] Signal code:  (-6)
[fv-az1493-330:08995] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe9abc42520]
[fv-az1493-330:08995] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe9abc969fc]
[fv-az1493-330:08995] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe9abc42476]
[fv-az1493-330:08995] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe9abc287f3]
[fv-az1493-330:08995] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fe9ac0a4f26]
[fv-az1493-330:08995] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fe9ac0b6d9c]
[fv-az1493-330:08995] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fe9ac0b6e07]
[fv-az1493-330:08995] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe9ac0b70bb]
[fv-az1493-330:08995] [ 8] plumed(+0x12f48)[0x55fe2ef05f48]
[fv-az1493-330:08995] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe9abc29d90]
[fv-az1493-330:08995] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe9abc29e40]
[fv-az1493-330:08995] [11] plumed(+0x131e5)[0x55fe2ef061e5]
[fv-az1493-330:08995] *** End of error message ***
</pre>
{% endraw %}

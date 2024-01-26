**Project ID:** [plumID:19.061]({{ '/' | absolute_url }}eggs/19/061/)  
Stderr for source:  ple_meta.dat   
Download: [zipped raw stdout](ple_meta.dat.plumed.stdout.txt.zip) - [zipped raw stderr](ple_meta.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : restart file HILLS not found
[fv-az1493-330:09026] *** Process received signal ***
[fv-az1493-330:09026] Signal: Aborted (6)
[fv-az1493-330:09026] Signal code:  (-6)
[fv-az1493-330:09026] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe758642520]
[fv-az1493-330:09026] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe7586969fc]
[fv-az1493-330:09026] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe758642476]
[fv-az1493-330:09026] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe7586287f3]
[fv-az1493-330:09026] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fe758aa4f26]
[fv-az1493-330:09026] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fe758ab6d9c]
[fv-az1493-330:09026] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fe758ab6e07]
[fv-az1493-330:09026] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe758ab70bb]
[fv-az1493-330:09026] [ 8] plumed(+0x12f48)[0x564ac2fa4f48]
[fv-az1493-330:09026] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe758629d90]
[fv-az1493-330:09026] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe758629e40]
[fv-az1493-330:09026] [11] plumed(+0x131e5)[0x564ac2fa51e5]
[fv-az1493-330:09026] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:20.007]({{ '/' | absolute_url }}eggs/20/007/)  
Stderr for source:  single/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : restart file HILLS not found
[fv-az1493-330:07604] *** Process received signal ***
[fv-az1493-330:07604] Signal: Aborted (6)
[fv-az1493-330:07604] Signal code:  (-6)
[fv-az1493-330:07604] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3f86e42520]
[fv-az1493-330:07604] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3f86e969fc]
[fv-az1493-330:07604] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3f86e42476]
[fv-az1493-330:07604] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3f86e287f3]
[fv-az1493-330:07604] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f3f872a4f26]
[fv-az1493-330:07604] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f3f872b6d9c]
[fv-az1493-330:07604] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f3f872b6e07]
[fv-az1493-330:07604] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3f872b70bb]
[fv-az1493-330:07604] [ 8] plumed(+0x12f48)[0x562e241f6f48]
[fv-az1493-330:07604] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3f86e29d90]
[fv-az1493-330:07604] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3f86e29e40]
[fv-az1493-330:07604] [11] plumed(+0x131e5)[0x562e241f71e5]
[fv-az1493-330:07604] *** End of error message ***
</pre>
{% endraw %}

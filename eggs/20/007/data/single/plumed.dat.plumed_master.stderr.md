**Project ID:** [plumID:20.007]({{ '/' | absolute_url }}eggs/20/007/)  
Stderr for source:  single/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : restart file HILLS not found
[fv-az1493-330:07612] *** Process received signal ***
[fv-az1493-330:07612] Signal: Aborted (6)
[fv-az1493-330:07612] Signal code:  (-6)
[fv-az1493-330:07612] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f03e9a42520]
[fv-az1493-330:07612] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f03e9a969fc]
[fv-az1493-330:07612] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f03e9a42476]
[fv-az1493-330:07612] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f03e9a287f3]
[fv-az1493-330:07612] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f03e9ea4f26]
[fv-az1493-330:07612] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f03e9eb6d9c]
[fv-az1493-330:07612] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f03e9eb6e07]
[fv-az1493-330:07612] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f03e9eb70bb]
[fv-az1493-330:07612] [ 8] plumed_master(+0x12ebf)[0x5628b3f43ebf]
[fv-az1493-330:07612] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f03e9a29d90]
[fv-az1493-330:07612] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f03e9a29e40]
[fv-az1493-330:07612] [11] plumed_master(+0x13155)[0x5628b3f44155]
[fv-az1493-330:07612] *** End of error message ***
</pre>
{% endraw %}

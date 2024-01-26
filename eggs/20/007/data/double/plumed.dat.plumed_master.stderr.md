**Project ID:** [plumID:20.007]({{ '/' | absolute_url }}eggs/20/007/)  
Stderr for source:  double/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : restart file HILLS not found
[fv-az1493-330:07581] *** Process received signal ***
[fv-az1493-330:07581] Signal: Aborted (6)
[fv-az1493-330:07581] Signal code:  (-6)
[fv-az1493-330:07581] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7321842520]
[fv-az1493-330:07581] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f73218969fc]
[fv-az1493-330:07581] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7321842476]
[fv-az1493-330:07581] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f73218287f3]
[fv-az1493-330:07581] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f7321ca4f26]
[fv-az1493-330:07581] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f7321cb6d9c]
[fv-az1493-330:07581] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f7321cb6e07]
[fv-az1493-330:07581] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7321cb70bb]
[fv-az1493-330:07581] [ 8] plumed_master(+0x12ebf)[0x560a6c70eebf]
[fv-az1493-330:07581] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7321829d90]
[fv-az1493-330:07581] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7321829e40]
[fv-az1493-330:07581] [11] plumed_master(+0x13155)[0x560a6c70f155]
[fv-az1493-330:07581] *** End of error message ***
</pre>
{% endraw %}

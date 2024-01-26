**Project ID:** [plumID:21.004]({{ '/' | absolute_url }}eggs/21/004/)  
Stderr for source:  HST-GST/CB8-G6/plumed_path.dat   
Download: [zipped raw stdout](plumed_path.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_path.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : restart file HILLS not found
[fv-az1542-52:07843] *** Process received signal ***
[fv-az1542-52:07843] Signal: Aborted (6)
[fv-az1542-52:07843] Signal code:  (-6)
[fv-az1542-52:07843] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb4fa442520]
[fv-az1542-52:07843] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb4fa4969fc]
[fv-az1542-52:07843] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb4fa442476]
[fv-az1542-52:07843] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb4fa4287f3]
[fv-az1542-52:07843] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fb4fa8a4f26]
[fv-az1542-52:07843] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fb4fa8b6d9c]
[fv-az1542-52:07843] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fb4fa8b6e07]
[fv-az1542-52:07843] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb4fa8b70bb]
[fv-az1542-52:07843] [ 8] plumed_master(+0x12ebf)[0x55e55fd01ebf]
[fv-az1542-52:07843] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb4fa429d90]
[fv-az1542-52:07843] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb4fa429e40]
[fv-az1542-52:07843] [11] plumed_master(+0x13155)[0x55e55fd02155]
[fv-az1542-52:07843] *** End of error message ***
</pre>
{% endraw %}

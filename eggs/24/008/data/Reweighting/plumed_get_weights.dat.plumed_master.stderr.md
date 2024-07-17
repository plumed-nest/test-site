**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  Reweighting/plumed_get_weights.dat   
Download: [zipped raw stdout](plumed_get_weights.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_get_weights.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label rho : could not find file named rtp_coord.dat
[fv-az1110-714:69403] *** Process received signal ***
[fv-az1110-714:69403] Signal: Aborted (6)
[fv-az1110-714:69403] Signal code:  (-6)
[fv-az1110-714:69403] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4f3ac42520]
[fv-az1110-714:69403] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4f3ac969fc]
[fv-az1110-714:69403] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4f3ac42476]
[fv-az1110-714:69403] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4f3ac287f3]
[fv-az1110-714:69403] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f4f3b0a2b9e]
[fv-az1110-714:69403] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f4f3b0ae20c]
[fv-az1110-714:69403] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f4f3b0ae277]
[fv-az1110-714:69403] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4f3b0ae52b]
[fv-az1110-714:69403] [ 8] plumed_master(+0x14274)[0x55ca80c11274]
[fv-az1110-714:69403] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4f3ac29d90]
[fv-az1110-714:69403] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4f3ac29e40]
[fv-az1110-714:69403] [11] plumed_master(+0x14ed5)[0x55ca80c11ed5]
[fv-az1110-714:69403] *** End of error message ***
</pre>
{% endraw %}

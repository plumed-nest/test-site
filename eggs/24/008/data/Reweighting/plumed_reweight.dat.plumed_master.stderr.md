**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  Reweighting/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label rho : could not find file named rtp_coord.dat
[fv-az1110-714:69434] *** Process received signal ***
[fv-az1110-714:69434] Signal: Aborted (6)
[fv-az1110-714:69434] Signal code:  (-6)
[fv-az1110-714:69434] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0017e42520]
[fv-az1110-714:69434] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0017e969fc]
[fv-az1110-714:69434] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0017e42476]
[fv-az1110-714:69434] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0017e287f3]
[fv-az1110-714:69434] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f00182a2b9e]
[fv-az1110-714:69434] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f00182ae20c]
[fv-az1110-714:69434] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f00182ae277]
[fv-az1110-714:69434] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f00182ae52b]
[fv-az1110-714:69434] [ 8] plumed_master(+0x14274)[0x55f61f66e274]
[fv-az1110-714:69434] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0017e29d90]
[fv-az1110-714:69434] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0017e29e40]
[fv-az1110-714:69434] [11] plumed_master(+0x14ed5)[0x55f61f66eed5]
[fv-az1110-714:69434] *** End of error message ***
</pre>
{% endraw %}
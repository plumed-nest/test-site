**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  Reweighting/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label rho : could not find file named rtp_coord.dat
[fv-az1110-714:69426] *** Process received signal ***
[fv-az1110-714:69426] Signal: Aborted (6)
[fv-az1110-714:69426] Signal code:  (-6)
[fv-az1110-714:69426] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdc36042520]
[fv-az1110-714:69426] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdc360969fc]
[fv-az1110-714:69426] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdc36042476]
[fv-az1110-714:69426] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdc360287f3]
[fv-az1110-714:69426] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fdc364a2b9e]
[fv-az1110-714:69426] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fdc364ae20c]
[fv-az1110-714:69426] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fdc364ae277]
[fv-az1110-714:69426] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdc364ae52b]
[fv-az1110-714:69426] [ 8] plumed(+0x12f48)[0x556a536b7f48]
[fv-az1110-714:69426] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdc36029d90]
[fv-az1110-714:69426] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdc36029e40]
[fv-az1110-714:69426] [11] plumed(+0x131e5)[0x556a536b81e5]
[fv-az1110-714:69426] *** End of error message ***
</pre>
{% endraw %}

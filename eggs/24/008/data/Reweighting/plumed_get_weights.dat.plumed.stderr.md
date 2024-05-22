**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  Reweighting/plumed_get_weights.dat   
Download: [zipped raw stdout](plumed_get_weights.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_get_weights.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label rho : could not find file named rtp_coord.dat
[fv-az1435-553:39063] *** Process received signal ***
[fv-az1435-553:39063] Signal: Aborted (6)
[fv-az1435-553:39063] Signal code:  (-6)
[fv-az1435-553:39063] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f04d8642520]
[fv-az1435-553:39063] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f04d86969fc]
[fv-az1435-553:39063] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f04d8642476]
[fv-az1435-553:39063] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f04d86287f3]
[fv-az1435-553:39063] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f04d8aa2b9e]
[fv-az1435-553:39063] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f04d8aae20c]
[fv-az1435-553:39063] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f04d8aae277]
[fv-az1435-553:39063] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f04d8aae52b]
[fv-az1435-553:39063] [ 8] plumed(+0x12f48)[0x5631daa0df48]
[fv-az1435-553:39063] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f04d8629d90]
[fv-az1435-553:39063] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f04d8629e40]
[fv-az1435-553:39063] [11] plumed(+0x131e5)[0x5631daa0e1e5]
[fv-az1435-553:39063] *** End of error message ***
</pre>
{% endraw %}

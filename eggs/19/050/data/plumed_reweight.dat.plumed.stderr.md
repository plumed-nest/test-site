**Project ID:** [plumID:19.050]({{ '/' | absolute_url }}eggs/19/050/)  
Stderr for source:  plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE_FROM_CONTOUR with label cont : keyword DATA is compulsory for this action
[fv-az1110-714:73572] *** Process received signal ***
[fv-az1110-714:73572] Signal: Aborted (6)
[fv-az1110-714:73572] Signal code:  (-6)
[fv-az1110-714:73572] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1e37642520]
[fv-az1110-714:73572] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1e376969fc]
[fv-az1110-714:73572] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1e37642476]
[fv-az1110-714:73572] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1e376287f3]
[fv-az1110-714:73572] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1e37aa2b9e]
[fv-az1110-714:73572] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1e37aae20c]
[fv-az1110-714:73572] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1e37aae277]
[fv-az1110-714:73572] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1e37aae52b]
[fv-az1110-714:73572] [ 8] plumed(+0x12f48)[0x5610c347cf48]
[fv-az1110-714:73572] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1e37629d90]
[fv-az1110-714:73572] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1e37629e40]
[fv-az1110-714:73572] [11] plumed(+0x131e5)[0x5610c347d1e5]
[fv-az1110-714:73572] *** End of error message ***
</pre>
{% endraw %}

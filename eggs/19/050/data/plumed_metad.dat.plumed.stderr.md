**Project ID:** [plumID:19.050]({{ '/' | absolute_url }}eggs/19/050/)  
Stderr for source:  plumed_metad.dat   
Download: [zipped raw stdout](plumed_metad.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_metad.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE_FROM_CONTOUR with label cont : keyword DATA is compulsory for this action
[fv-az1110-714:73542] *** Process received signal ***
[fv-az1110-714:73542] Signal: Aborted (6)
[fv-az1110-714:73542] Signal code:  (-6)
[fv-az1110-714:73542] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0efca42520]
[fv-az1110-714:73542] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0efca969fc]
[fv-az1110-714:73542] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0efca42476]
[fv-az1110-714:73542] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0efca287f3]
[fv-az1110-714:73542] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f0efcea2b9e]
[fv-az1110-714:73542] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f0efceae20c]
[fv-az1110-714:73542] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f0efceae277]
[fv-az1110-714:73542] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f0efceae52b]
[fv-az1110-714:73542] [ 8] plumed(+0x12f48)[0x55a8f0577f48]
[fv-az1110-714:73542] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0efca29d90]
[fv-az1110-714:73542] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0efca29e40]
[fv-az1110-714:73542] [11] plumed(+0x131e5)[0x55a8f05781e5]
[fv-az1110-714:73542] *** End of error message ***
</pre>
{% endraw %}

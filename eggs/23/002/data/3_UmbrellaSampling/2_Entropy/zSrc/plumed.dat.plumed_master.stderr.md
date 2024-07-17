**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  3_UmbrellaSampling/2_Entropy/zSrc/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action PAIRENTROPY with label @s13 : keyword GRID_BIN is compulsory for this action
[fv-az774-16:70554] *** Process received signal ***
[fv-az774-16:70554] Signal: Aborted (6)
[fv-az774-16:70554] Signal code:  (-6)
[fv-az774-16:70554] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f86caa42520]
[fv-az774-16:70554] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f86caa969fc]
[fv-az774-16:70554] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f86caa42476]
[fv-az774-16:70554] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f86caa287f3]
[fv-az774-16:70554] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f86caea2b9e]
[fv-az774-16:70554] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f86caeae20c]
[fv-az774-16:70554] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f86caeae277]
[fv-az774-16:70554] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f86caeae52b]
[fv-az774-16:70554] [ 8] plumed_master(+0x14274)[0x55d7505e0274]
[fv-az774-16:70554] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f86caa29d90]
[fv-az774-16:70554] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f86caa29e40]
[fv-az774-16:70554] [11] plumed_master(+0x14ed5)[0x55d7505e0ed5]
[fv-az774-16:70554] *** End of error message ***
</pre>
{% endraw %}

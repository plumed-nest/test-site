**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_for_reference_map.dat   
Download: [zipped raw stdout](plumed_for_reference_map.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_for_reference_map.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action VSTACK with label mat : no arguments were specificed
[fv-az975-63:70133] *** Process received signal ***
[fv-az975-63:70133] Signal: Aborted (6)
[fv-az975-63:70133] Signal code:  (-6)
[fv-az975-63:70133] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5d2bc42520]
[fv-az975-63:70133] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5d2bc969fc]
[fv-az975-63:70133] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5d2bc42476]
[fv-az975-63:70133] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5d2bc287f3]
[fv-az975-63:70133] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f5d2c0a2b9e]
[fv-az975-63:70133] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f5d2c0ae20c]
[fv-az975-63:70133] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f5d2c0ae277]
[fv-az975-63:70133] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5d2c0ae52b]
[fv-az975-63:70133] [ 8] plumed_master(+0x14274)[0x55de192f3274]
[fv-az975-63:70133] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5d2bc29d90]
[fv-az975-63:70133] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5d2bc29e40]
[fv-az975-63:70133] [11] plumed_master(+0x14ed5)[0x55de192f3ed5]
[fv-az975-63:70133] *** End of error message ***
</pre>
{% endraw %}

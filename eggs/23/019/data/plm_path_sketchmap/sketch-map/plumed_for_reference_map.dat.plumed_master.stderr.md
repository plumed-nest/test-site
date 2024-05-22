**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_for_reference_map.dat   
Download: [zipped raw stdout](plumed_for_reference_map.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_for_reference_map.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action VSTACK with label mat : no arguments were specificed
[fv-az1106-239:39588] *** Process received signal ***
[fv-az1106-239:39588] Signal: Aborted (6)
[fv-az1106-239:39588] Signal code:  (-6)
[fv-az1106-239:39588] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f749c442520]
[fv-az1106-239:39588] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f749c4969fc]
[fv-az1106-239:39588] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f749c442476]
[fv-az1106-239:39588] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f749c4287f3]
[fv-az1106-239:39588] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f749c8a2b9e]
[fv-az1106-239:39588] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f749c8ae20c]
[fv-az1106-239:39588] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f749c8ae277]
[fv-az1106-239:39588] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f749c8ae52b]
[fv-az1106-239:39588] [ 8] plumed_master(+0x14274)[0x5645f3dd2274]
[fv-az1106-239:39588] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f749c429d90]
[fv-az1106-239:39588] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f749c429e40]
[fv-az1106-239:39588] [11] plumed_master(+0x14ed5)[0x5645f3dd2ed5]
[fv-az1106-239:39588] *** End of error message ***
</pre>
{% endraw %}

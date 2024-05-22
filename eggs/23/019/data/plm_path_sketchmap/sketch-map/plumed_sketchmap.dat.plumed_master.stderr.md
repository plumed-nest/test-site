**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_sketchmap.dat   
Download: [zipped raw stdout](plumed_sketchmap.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_sketchmap.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action VSTACK with label mat : no arguments were specificed
[fv-az1106-239:39651] *** Process received signal ***
[fv-az1106-239:39651] Signal: Aborted (6)
[fv-az1106-239:39651] Signal code:  (-6)
[fv-az1106-239:39651] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa1cca42520]
[fv-az1106-239:39651] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa1cca969fc]
[fv-az1106-239:39651] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa1cca42476]
[fv-az1106-239:39651] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa1cca287f3]
[fv-az1106-239:39651] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa1ccea2b9e]
[fv-az1106-239:39651] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa1cceae20c]
[fv-az1106-239:39651] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa1cceae277]
[fv-az1106-239:39651] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa1cceae52b]
[fv-az1106-239:39651] [ 8] plumed_master(+0x14274)[0x5642d3dc2274]
[fv-az1106-239:39651] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa1cca29d90]
[fv-az1106-239:39651] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa1cca29e40]
[fv-az1106-239:39651] [11] plumed_master(+0x14ed5)[0x5642d3dc2ed5]
[fv-az1106-239:39651] *** End of error message ***
</pre>
{% endraw %}

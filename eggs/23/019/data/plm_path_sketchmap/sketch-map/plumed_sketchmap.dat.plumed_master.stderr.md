**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_sketchmap.dat   
Download: [zipped raw stdout](plumed_sketchmap.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_sketchmap.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action VSTACK with label mat : no arguments were specificed
[fv-az975-63:70195] *** Process received signal ***
[fv-az975-63:70195] Signal: Aborted (6)
[fv-az975-63:70195] Signal code:  (-6)
[fv-az975-63:70195] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1cff042520]
[fv-az975-63:70195] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1cff0969fc]
[fv-az975-63:70195] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1cff042476]
[fv-az975-63:70195] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1cff0287f3]
[fv-az975-63:70195] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1cff4a2b9e]
[fv-az975-63:70195] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1cff4ae20c]
[fv-az975-63:70195] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1cff4ae277]
[fv-az975-63:70195] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1cff4ae52b]
[fv-az975-63:70195] [ 8] plumed_master(+0x14274)[0x55b0bc84e274]
[fv-az975-63:70195] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1cff029d90]
[fv-az975-63:70195] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1cff029e40]
[fv-az975-63:70195] [11] plumed_master(+0x14ed5)[0x55b0bc84eed5]
[fv-az975-63:70195] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/atlas_3d/res/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az1543-369:41467] *** Process received signal ***
[fv-az1543-369:41467] Signal: Aborted (6)
[fv-az1543-369:41467] Signal code:  (-6)
[fv-az1543-369:41467] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fbd46642520]
[fv-az1543-369:41467] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fbd466969fc]
[fv-az1543-369:41467] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fbd46642476]
[fv-az1543-369:41467] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fbd466287f3]
[fv-az1543-369:41467] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fbd46aa2b9e]
[fv-az1543-369:41467] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fbd46aae20c]
[fv-az1543-369:41467] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fbd46aae277]
[fv-az1543-369:41467] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fbd46aae52b]
[fv-az1543-369:41467] [ 8] plumed_master(+0x14274)[0x55ec3d575274]
[fv-az1543-369:41467] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fbd46629d90]
[fv-az1543-369:41467] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fbd46629e40]
[fv-az1543-369:41467] [11] plumed_master(+0x14ed5)[0x55ec3d575ed5]
[fv-az1543-369:41467] *** End of error message ***
</pre>
{% endraw %}

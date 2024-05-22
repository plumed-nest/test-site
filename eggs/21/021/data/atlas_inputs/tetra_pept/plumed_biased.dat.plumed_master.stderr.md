**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/tetra_pept/plumed_biased.dat   
Download: [zipped raw stdout](plumed_biased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_biased.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az1543-369:41625] *** Process received signal ***
[fv-az1543-369:41625] Signal: Aborted (6)
[fv-az1543-369:41625] Signal code:  (-6)
[fv-az1543-369:41625] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8751842520]
[fv-az1543-369:41625] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f87518969fc]
[fv-az1543-369:41625] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8751842476]
[fv-az1543-369:41625] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f87518287f3]
[fv-az1543-369:41625] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8751ca2b9e]
[fv-az1543-369:41625] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8751cae20c]
[fv-az1543-369:41625] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8751cae277]
[fv-az1543-369:41625] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8751cae52b]
[fv-az1543-369:41625] [ 8] plumed_master(+0x14274)[0x5578cc14a274]
[fv-az1543-369:41625] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8751829d90]
[fv-az1543-369:41625] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8751829e40]
[fv-az1543-369:41625] [11] plumed_master(+0x14ed5)[0x5578cc14aed5]
[fv-az1543-369:41625] *** End of error message ***
</pre>
{% endraw %}

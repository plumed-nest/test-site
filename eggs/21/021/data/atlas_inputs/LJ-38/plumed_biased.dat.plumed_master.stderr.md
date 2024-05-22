**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/LJ-38/plumed_biased.dat   
Download: [zipped raw stdout](plumed_biased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_biased.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az1543-369:41312] *** Process received signal ***
[fv-az1543-369:41312] Signal: Aborted (6)
[fv-az1543-369:41312] Signal code:  (-6)
[fv-az1543-369:41312] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb941442520]
[fv-az1543-369:41312] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb9414969fc]
[fv-az1543-369:41312] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb941442476]
[fv-az1543-369:41312] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb9414287f3]
[fv-az1543-369:41312] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb9418a2b9e]
[fv-az1543-369:41312] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb9418ae20c]
[fv-az1543-369:41312] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb9418ae277]
[fv-az1543-369:41312] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb9418ae52b]
[fv-az1543-369:41312] [ 8] plumed_master(+0x14274)[0x563d52824274]
[fv-az1543-369:41312] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb941429d90]
[fv-az1543-369:41312] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb941429e40]
[fv-az1543-369:41312] [11] plumed_master(+0x14ed5)[0x563d52824ed5]
[fv-az1543-369:41312] *** End of error message ***
</pre>
{% endraw %}

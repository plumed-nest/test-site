**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/atlas_3d/pca_2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az1543-369:41436] *** Process received signal ***
[fv-az1543-369:41436] Signal: Aborted (6)
[fv-az1543-369:41436] Signal code:  (-6)
[fv-az1543-369:41436] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb69fe42520]
[fv-az1543-369:41436] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb69fe969fc]
[fv-az1543-369:41436] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb69fe42476]
[fv-az1543-369:41436] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb69fe287f3]
[fv-az1543-369:41436] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb6a02a2b9e]
[fv-az1543-369:41436] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb6a02ae20c]
[fv-az1543-369:41436] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb6a02ae277]
[fv-az1543-369:41436] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb6a02ae52b]
[fv-az1543-369:41436] [ 8] plumed_master(+0x14274)[0x556fab1f8274]
[fv-az1543-369:41436] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb69fe29d90]
[fv-az1543-369:41436] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb69fe29e40]
[fv-az1543-369:41436] [11] plumed_master(+0x14ed5)[0x556fab1f8ed5]
[fv-az1543-369:41436] *** End of error message ***
</pre>
{% endraw %}

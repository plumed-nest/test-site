**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/atlas_6d/pca_2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az1543-369:41531] *** Process received signal ***
[fv-az1543-369:41531] Signal: Aborted (6)
[fv-az1543-369:41531] Signal code:  (-6)
[fv-az1543-369:41531] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f335ee42520]
[fv-az1543-369:41531] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f335ee969fc]
[fv-az1543-369:41531] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f335ee42476]
[fv-az1543-369:41531] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f335ee287f3]
[fv-az1543-369:41531] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f335f2a2b9e]
[fv-az1543-369:41531] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f335f2ae20c]
[fv-az1543-369:41531] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f335f2ae277]
[fv-az1543-369:41531] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f335f2ae52b]
[fv-az1543-369:41531] [ 8] plumed_master(+0x14274)[0x55589a5d5274]
[fv-az1543-369:41531] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f335ee29d90]
[fv-az1543-369:41531] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f335ee29e40]
[fv-az1543-369:41531] [11] plumed_master(+0x14ed5)[0x55589a5d5ed5]
[fv-az1543-369:41531] *** End of error message ***
</pre>
{% endraw %}

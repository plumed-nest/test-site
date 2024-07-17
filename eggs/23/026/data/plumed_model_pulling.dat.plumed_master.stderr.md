**Project ID:** [plumID:23.026]({{ '/' | absolute_url }}eggs/23/026/)  
Stderr for source:  plumed_model_pulling.dat   
Download: [zipped raw stdout](plumed_model_pulling.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_model_pulling.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az841-65:69623] *** Process received signal ***
[fv-az841-65:69623] Signal: Aborted (6)
[fv-az841-65:69623] Signal code:  (-6)
[fv-az841-65:69623] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7462042520]
[fv-az841-65:69623] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f74620969fc]
[fv-az841-65:69623] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7462042476]
[fv-az841-65:69623] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f74620287f3]
[fv-az841-65:69623] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f74624a2b9e]
[fv-az841-65:69623] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f74624ae20c]
[fv-az841-65:69623] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f74624ae277]
[fv-az841-65:69623] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f74624ae52b]
[fv-az841-65:69623] [ 8] plumed_master(+0x14274)[0x562361250274]
[fv-az841-65:69623] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7462029d90]
[fv-az841-65:69623] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7462029e40]
[fv-az841-65:69623] [11] plumed_master(+0x14ed5)[0x562361250ed5]
[fv-az841-65:69623] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-jax2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az659-178:71746] *** Process received signal ***
[fv-az659-178:71746] Signal: Aborted (6)
[fv-az659-178:71746] Signal code:  (-6)
[fv-az659-178:71746] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7eff8d042520]
[fv-az659-178:71746] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7eff8d0969fc]
[fv-az659-178:71746] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7eff8d042476]
[fv-az659-178:71746] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7eff8d0287f3]
[fv-az659-178:71746] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7eff8d4a2b9e]
[fv-az659-178:71746] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7eff8d4ae20c]
[fv-az659-178:71746] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7eff8d4ae277]
[fv-az659-178:71746] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7eff8d4ae52b]
[fv-az659-178:71746] [ 8] plumed_master(+0x14274)[0x557a856d4274]
[fv-az659-178:71746] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7eff8d029d90]
[fv-az659-178:71746] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7eff8d029e40]
[fv-az659-178:71746] [11] plumed_master(+0x14ed5)[0x557a856d4ed5]
[fv-az659-178:71746] *** End of error message ***
</pre>
{% endraw %}
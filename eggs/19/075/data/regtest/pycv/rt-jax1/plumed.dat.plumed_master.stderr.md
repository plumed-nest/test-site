**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-jax1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az1109-238:41452] *** Process received signal ***
[fv-az1109-238:41452] Signal: Aborted (6)
[fv-az1109-238:41452] Signal code:  (-6)
[fv-az1109-238:41452] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe1c6242520]
[fv-az1109-238:41452] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe1c62969fc]
[fv-az1109-238:41452] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe1c6242476]
[fv-az1109-238:41452] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe1c62287f3]
[fv-az1109-238:41452] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fe1c66a2b9e]
[fv-az1109-238:41452] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fe1c66ae20c]
[fv-az1109-238:41452] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fe1c66ae277]
[fv-az1109-238:41452] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe1c66ae52b]
[fv-az1109-238:41452] [ 8] plumed_master(+0x14274)[0x5617f2a2c274]
[fv-az1109-238:41452] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe1c6229d90]
[fv-az1109-238:41452] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe1c6229e40]
[fv-az1109-238:41452] [11] plumed_master(+0x14ed5)[0x5617f2a2ced5]
[fv-az1109-238:41452] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w25-s6.492/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az774-16:72550] *** Process received signal ***
[fv-az774-16:72550] Signal: Aborted (6)
[fv-az774-16:72550] Signal code:  (-6)
[fv-az774-16:72550] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f82f5a42520]
[fv-az774-16:72550] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f82f5a969fc]
[fv-az774-16:72550] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f82f5a42476]
[fv-az774-16:72550] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f82f5a287f3]
[fv-az774-16:72550] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f82f5ea2b9e]
[fv-az774-16:72550] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f82f5eae20c]
[fv-az774-16:72550] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f82f5eae277]
[fv-az774-16:72550] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f82f5eae52b]
[fv-az774-16:72550] [ 8] plumed_master(+0x14274)[0x56113d46a274]
[fv-az774-16:72550] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f82f5a29d90]
[fv-az774-16:72550] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f82f5a29e40]
[fv-az774-16:72550] [11] plumed_master(+0x14ed5)[0x56113d46aed5]
[fv-az774-16:72550] *** End of error message ***
</pre>
{% endraw %}

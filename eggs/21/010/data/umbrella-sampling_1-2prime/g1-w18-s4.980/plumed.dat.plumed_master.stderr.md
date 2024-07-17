**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w18-s4.980/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az774-16:72299] *** Process received signal ***
[fv-az774-16:72299] Signal: Aborted (6)
[fv-az774-16:72299] Signal code:  (-6)
[fv-az774-16:72299] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ff485c42520]
[fv-az774-16:72299] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ff485c969fc]
[fv-az774-16:72299] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ff485c42476]
[fv-az774-16:72299] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ff485c287f3]
[fv-az774-16:72299] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7ff4860a2b9e]
[fv-az774-16:72299] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7ff4860ae20c]
[fv-az774-16:72299] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7ff4860ae277]
[fv-az774-16:72299] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ff4860ae52b]
[fv-az774-16:72299] [ 8] plumed_master(+0x14274)[0x563bb70f4274]
[fv-az774-16:72299] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ff485c29d90]
[fv-az774-16:72299] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ff485c29e40]
[fv-az774-16:72299] [11] plumed_master(+0x14ed5)[0x563bb70f4ed5]
[fv-az774-16:72299] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_tor.dat   
Download: [zipped raw stdout](plumed_tor.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_tor.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az695-456:74675] *** Process received signal ***
[fv-az695-456:74675] Signal: Aborted (6)
[fv-az695-456:74675] Signal code:  (-6)
[fv-az695-456:74675] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2a10a42520]
[fv-az695-456:74675] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2a10a969fc]
[fv-az695-456:74675] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2a10a42476]
[fv-az695-456:74675] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2a10a287f3]
[fv-az695-456:74675] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f2a10ea2b9e]
[fv-az695-456:74675] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f2a10eae20c]
[fv-az695-456:74675] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f2a10eae277]
[fv-az695-456:74675] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f2a10eae52b]
[fv-az695-456:74675] [ 8] plumed_master(+0x14274)[0x55c19f542274]
[fv-az695-456:74675] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2a10a29d90]
[fv-az695-456:74675] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2a10a29e40]
[fv-az695-456:74675] [11] plumed_master(+0x14ed5)[0x55c19f542ed5]
[fv-az695-456:74675] *** End of error message ***
</pre>
{% endraw %}
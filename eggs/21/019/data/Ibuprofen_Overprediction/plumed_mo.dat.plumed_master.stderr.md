**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_mo.dat   
Download: [zipped raw stdout](plumed_mo.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_mo.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az695-456:74644] *** Process received signal ***
[fv-az695-456:74644] Signal: Aborted (6)
[fv-az695-456:74644] Signal code:  (-6)
[fv-az695-456:74644] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7efe1b642520]
[fv-az695-456:74644] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7efe1b6969fc]
[fv-az695-456:74644] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7efe1b642476]
[fv-az695-456:74644] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7efe1b6287f3]
[fv-az695-456:74644] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7efe1baa2b9e]
[fv-az695-456:74644] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7efe1baae20c]
[fv-az695-456:74644] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7efe1baae277]
[fv-az695-456:74644] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7efe1baae52b]
[fv-az695-456:74644] [ 8] plumed_master(+0x14274)[0x55567c575274]
[fv-az695-456:74644] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7efe1b629d90]
[fv-az695-456:74644] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7efe1b629e40]
[fv-az695-456:74644] [11] plumed_master(+0x14ed5)[0x55567c575ed5]
[fv-az695-456:74644] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:24.009]({{ '/' | absolute_url }}eggs/24/009/)  
Stderr for source:  actin_lda_setup/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az2031-223:39085] *** Process received signal ***
[fv-az2031-223:39085] Signal: Aborted (6)
[fv-az2031-223:39085] Signal code:  (-6)
[fv-az2031-223:39085] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1472642520]
[fv-az2031-223:39085] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f14726969fc]
[fv-az2031-223:39085] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1472642476]
[fv-az2031-223:39085] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f14726287f3]
[fv-az2031-223:39085] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1472aa2b9e]
[fv-az2031-223:39085] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1472aae20c]
[fv-az2031-223:39085] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1472aae277]
[fv-az2031-223:39085] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1472aae52b]
[fv-az2031-223:39085] [ 8] plumed_master(+0x14274)[0x5623679bb274]
[fv-az2031-223:39085] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1472629d90]
[fv-az2031-223:39085] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1472629e40]
[fv-az2031-223:39085] [11] plumed_master(+0x14ed5)[0x5623679bbed5]
[fv-az2031-223:39085] *** End of error message ***
</pre>
{% endraw %}

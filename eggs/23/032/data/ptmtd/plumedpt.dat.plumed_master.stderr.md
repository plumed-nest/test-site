**Project ID:** [plumID:23.032]({{ '/' | absolute_url }}eggs/23/032/)  
Stderr for source:  ptmtd/plumedpt.dat   
Download: [zipped raw stdout](plumedpt.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumedpt.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az774-16:69685] *** Process received signal ***
[fv-az774-16:69685] Signal: Aborted (6)
[fv-az774-16:69685] Signal code:  (-6)
[fv-az774-16:69685] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe7e8842520]
[fv-az774-16:69685] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe7e88969fc]
[fv-az774-16:69685] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe7e8842476]
[fv-az774-16:69685] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe7e88287f3]
[fv-az774-16:69685] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fe7e8ca2b9e]
[fv-az774-16:69685] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fe7e8cae20c]
[fv-az774-16:69685] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fe7e8cae277]
[fv-az774-16:69685] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe7e8cae52b]
[fv-az774-16:69685] [ 8] plumed_master(+0x14274)[0x559c9b1c2274]
[fv-az774-16:69685] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe7e8829d90]
[fv-az774-16:69685] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe7e8829e40]
[fv-az774-16:69685] [11] plumed_master(+0x14ed5)[0x559c9b1c2ed5]
[fv-az774-16:69685] *** End of error message ***
</pre>
{% endraw %}

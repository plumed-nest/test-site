**Project ID:** [plumID:23.043]({{ '/' | absolute_url }}eggs/23/043/)  
Stderr for source:  metad-example/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az774-16:69549] *** Process received signal ***
[fv-az774-16:69549] Signal: Aborted (6)
[fv-az774-16:69549] Signal code:  (-6)
[fv-az774-16:69549] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ff99d442520]
[fv-az774-16:69549] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ff99d4969fc]
[fv-az774-16:69549] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ff99d442476]
[fv-az774-16:69549] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ff99d4287f3]
[fv-az774-16:69549] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7ff99d8a2b9e]
[fv-az774-16:69549] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7ff99d8ae20c]
[fv-az774-16:69549] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7ff99d8ae277]
[fv-az774-16:69549] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ff99d8ae52b]
[fv-az774-16:69549] [ 8] plumed_master(+0x14274)[0x5629a0dfa274]
[fv-az774-16:69549] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ff99d429d90]
[fv-az774-16:69549] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ff99d429e40]
[fv-az774-16:69549] [11] plumed_master(+0x14ed5)[0x5629a0dfaed5]
[fv-az774-16:69549] *** End of error message ***
</pre>
{% endraw %}
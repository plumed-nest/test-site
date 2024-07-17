**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  FFH_scripts/plumed_FFH.dat   
Download: [zipped raw stdout](plumed_FFH.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_FFH.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az1110-714:71549] *** Process received signal ***
[fv-az1110-714:71549] Signal: Aborted (6)
[fv-az1110-714:71549] Signal code:  (-6)
[fv-az1110-714:71549] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6769042520]
[fv-az1110-714:71549] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f67690969fc]
[fv-az1110-714:71549] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6769042476]
[fv-az1110-714:71549] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f67690287f3]
[fv-az1110-714:71549] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f67694a2b9e]
[fv-az1110-714:71549] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f67694ae20c]
[fv-az1110-714:71549] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f67694ae277]
[fv-az1110-714:71549] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f67694ae52b]
[fv-az1110-714:71549] [ 8] plumed_master(+0x14274)[0x557d06c25274]
[fv-az1110-714:71549] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6769029d90]
[fv-az1110-714:71549] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6769029e40]
[fv-az1110-714:71549] [11] plumed_master(+0x14ed5)[0x557d06c25ed5]
[fv-az1110-714:71549] *** End of error message ***
</pre>
{% endraw %}

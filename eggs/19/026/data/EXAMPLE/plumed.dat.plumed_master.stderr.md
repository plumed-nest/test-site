**Project ID:** [plumID:19.026]({{ '/' | absolute_url }}eggs/19/026/)  
Stderr for source:  EXAMPLE/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az975-63:75882] *** Process received signal ***
[fv-az975-63:75882] Signal: Aborted (6)
[fv-az975-63:75882] Signal code:  (-6)
[fv-az975-63:75882] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe8afc42520]
[fv-az975-63:75882] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe8afc969fc]
[fv-az975-63:75882] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe8afc42476]
[fv-az975-63:75882] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe8afc287f3]
[fv-az975-63:75882] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fe8b00a2b9e]
[fv-az975-63:75882] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fe8b00ae20c]
[fv-az975-63:75882] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fe8b00ae277]
[fv-az975-63:75882] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe8b00ae52b]
[fv-az975-63:75882] [ 8] plumed_master(+0x14274)[0x55c576249274]
[fv-az975-63:75882] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe8afc29d90]
[fv-az975-63:75882] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe8afc29e40]
[fv-az975-63:75882] [11] plumed_master(+0x14ed5)[0x55c576249ed5]
[fv-az975-63:75882] *** End of error message ***
</pre>
{% endraw %}

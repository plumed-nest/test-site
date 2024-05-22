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
[fv-az1435-553:39095] *** Process received signal ***
[fv-az1435-553:39095] Signal: Aborted (6)
[fv-az1435-553:39095] Signal code:  (-6)
[fv-az1435-553:39095] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb624842520]
[fv-az1435-553:39095] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb6248969fc]
[fv-az1435-553:39095] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb624842476]
[fv-az1435-553:39095] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb6248287f3]
[fv-az1435-553:39095] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb624ca2b9e]
[fv-az1435-553:39095] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb624cae20c]
[fv-az1435-553:39095] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb624cae277]
[fv-az1435-553:39095] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb624cae52b]
[fv-az1435-553:39095] [ 8] plumed_master(+0x14274)[0x56034a40f274]
[fv-az1435-553:39095] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb624829d90]
[fv-az1435-553:39095] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb624829e40]
[fv-az1435-553:39095] [11] plumed_master(+0x14ed5)[0x56034a40fed5]
[fv-az1435-553:39095] *** End of error message ***
</pre>
{% endraw %}

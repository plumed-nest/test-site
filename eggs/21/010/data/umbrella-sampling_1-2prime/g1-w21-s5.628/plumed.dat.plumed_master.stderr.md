**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w21-s5.628/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az1435-553:42041] *** Process received signal ***
[fv-az1435-553:42041] Signal: Aborted (6)
[fv-az1435-553:42041] Signal code:  (-6)
[fv-az1435-553:42041] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6113c42520]
[fv-az1435-553:42041] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6113c969fc]
[fv-az1435-553:42041] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6113c42476]
[fv-az1435-553:42041] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6113c287f3]
[fv-az1435-553:42041] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f61140a2b9e]
[fv-az1435-553:42041] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f61140ae20c]
[fv-az1435-553:42041] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f61140ae277]
[fv-az1435-553:42041] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f61140ae52b]
[fv-az1435-553:42041] [ 8] plumed_master(+0x14274)[0x558ceb651274]
[fv-az1435-553:42041] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6113c29d90]
[fv-az1435-553:42041] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6113c29e40]
[fv-az1435-553:42041] [11] plumed_master(+0x14ed5)[0x558ceb651ed5]
[fv-az1435-553:42041] *** End of error message ***
</pre>
{% endraw %}

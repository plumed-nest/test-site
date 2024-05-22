**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w12-s3.684/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az1435-553:41728] *** Process received signal ***
[fv-az1435-553:41728] Signal: Aborted (6)
[fv-az1435-553:41728] Signal code:  (-6)
[fv-az1435-553:41728] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdcb6042520]
[fv-az1435-553:41728] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdcb60969fc]
[fv-az1435-553:41728] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdcb6042476]
[fv-az1435-553:41728] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdcb60287f3]
[fv-az1435-553:41728] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fdcb64a2b9e]
[fv-az1435-553:41728] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fdcb64ae20c]
[fv-az1435-553:41728] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fdcb64ae277]
[fv-az1435-553:41728] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdcb64ae52b]
[fv-az1435-553:41728] [ 8] plumed_master(+0x14274)[0x562f9ba9b274]
[fv-az1435-553:41728] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdcb6029d90]
[fv-az1435-553:41728] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdcb6029e40]
[fv-az1435-553:41728] [11] plumed_master(+0x14ed5)[0x562f9ba9bed5]
[fv-az1435-553:41728] *** End of error message ***
</pre>
{% endraw %}

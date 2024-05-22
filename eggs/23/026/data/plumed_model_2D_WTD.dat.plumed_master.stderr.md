**Project ID:** [plumID:23.026]({{ '/' | absolute_url }}eggs/23/026/)  
Stderr for source:  plumed_model_2D_WTD.dat   
Download: [zipped raw stdout](plumed_model_2D_WTD.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_model_2D_WTD.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az659-568:39203] *** Process received signal ***
[fv-az659-568:39203] Signal: Aborted (6)
[fv-az659-568:39203] Signal code:  (-6)
[fv-az659-568:39203] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1033c42520]
[fv-az659-568:39203] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1033c969fc]
[fv-az659-568:39203] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1033c42476]
[fv-az659-568:39203] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1033c287f3]
[fv-az659-568:39203] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f10340a2b9e]
[fv-az659-568:39203] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f10340ae20c]
[fv-az659-568:39203] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f10340ae277]
[fv-az659-568:39203] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f10340ae52b]
[fv-az659-568:39203] [ 8] plumed_master(+0x14274)[0x5569e76d7274]
[fv-az659-568:39203] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1033c29d90]
[fv-az659-568:39203] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1033c29e40]
[fv-az659-568:39203] [11] plumed_master(+0x14ed5)[0x5569e76d7ed5]
[fv-az659-568:39203] *** End of error message ***
</pre>
{% endraw %}

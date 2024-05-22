**Project ID:** [plumID:23.026]({{ '/' | absolute_url }}eggs/23/026/)  
Stderr for source:  plumed_model_pulling.dat   
Download: [zipped raw stdout](plumed_model_pulling.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_model_pulling.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az659-568:39235] *** Process received signal ***
[fv-az659-568:39235] Signal: Aborted (6)
[fv-az659-568:39235] Signal code:  (-6)
[fv-az659-568:39235] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7031842520]
[fv-az659-568:39235] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f70318969fc]
[fv-az659-568:39235] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7031842476]
[fv-az659-568:39235] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f70318287f3]
[fv-az659-568:39235] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f7031ca2b9e]
[fv-az659-568:39235] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f7031cae20c]
[fv-az659-568:39235] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f7031cae277]
[fv-az659-568:39235] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7031cae52b]
[fv-az659-568:39235] [ 8] plumed_master(+0x14274)[0x55dd52452274]
[fv-az659-568:39235] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7031829d90]
[fv-az659-568:39235] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7031829e40]
[fv-az659-568:39235] [11] plumed_master(+0x14ed5)[0x55dd52452ed5]
[fv-az659-568:39235] *** End of error message ***
</pre>
{% endraw %}

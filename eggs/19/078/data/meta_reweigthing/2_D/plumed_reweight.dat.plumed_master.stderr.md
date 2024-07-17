**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/2_D/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az695-456:75568] *** Process received signal ***
[fv-az695-456:75568] Signal: Aborted (6)
[fv-az695-456:75568] Signal code:  (-6)
[fv-az695-456:75568] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f545fe42520]
[fv-az695-456:75568] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f545fe969fc]
[fv-az695-456:75568] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f545fe42476]
[fv-az695-456:75568] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f545fe287f3]
[fv-az695-456:75568] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f54602a2b9e]
[fv-az695-456:75568] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f54602ae20c]
[fv-az695-456:75568] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f54602ae277]
[fv-az695-456:75568] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f54602ae52b]
[fv-az695-456:75568] [ 8] plumed_master(+0x14274)[0x55e44ed24274]
[fv-az695-456:75568] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f545fe29d90]
[fv-az695-456:75568] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f545fe29e40]
[fv-az695-456:75568] [11] plumed_master(+0x14ed5)[0x55e44ed24ed5]
[fv-az695-456:75568] *** End of error message ***
</pre>
{% endraw %}

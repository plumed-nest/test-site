**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/6_D/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az695-456:75749] *** Process received signal ***
[fv-az695-456:75749] Signal: Aborted (6)
[fv-az695-456:75749] Signal code:  (-6)
[fv-az695-456:75749] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f77ec242520]
[fv-az695-456:75749] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f77ec2969fc]
[fv-az695-456:75749] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f77ec242476]
[fv-az695-456:75749] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f77ec2287f3]
[fv-az695-456:75749] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f77ec6a2b9e]
[fv-az695-456:75749] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f77ec6ae20c]
[fv-az695-456:75749] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f77ec6ae277]
[fv-az695-456:75749] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f77ec6ae52b]
[fv-az695-456:75749] [ 8] plumed_master(+0x14274)[0x55d344c2d274]
[fv-az695-456:75749] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f77ec229d90]
[fv-az695-456:75749] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f77ec229e40]
[fv-az695-456:75749] [11] plumed_master(+0x14ed5)[0x55d344c2ded5]
[fv-az695-456:75749] *** End of error message ***
</pre>
{% endraw %}

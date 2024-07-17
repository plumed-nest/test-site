**Project ID:** [plumID:24.009]({{ '/' | absolute_url }}eggs/24/009/)  
Stderr for source:  actin_lda_setup/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az1445-962:69409] *** Process received signal ***
[fv-az1445-962:69409] Signal: Aborted (6)
[fv-az1445-962:69409] Signal code:  (-6)
[fv-az1445-962:69409] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2ed9442520]
[fv-az1445-962:69409] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2ed94969fc]
[fv-az1445-962:69409] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2ed9442476]
[fv-az1445-962:69409] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2ed94287f3]
[fv-az1445-962:69409] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f2ed98a2b9e]
[fv-az1445-962:69409] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f2ed98ae20c]
[fv-az1445-962:69409] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f2ed98ae277]
[fv-az1445-962:69409] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f2ed98ae52b]
[fv-az1445-962:69409] [ 8] plumed_master(+0x14274)[0x55e90d84b274]
[fv-az1445-962:69409] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2ed9429d90]
[fv-az1445-962:69409] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2ed9429e40]
[fv-az1445-962:69409] [11] plumed_master(+0x14ed5)[0x55e90d84bed5]
[fv-az1445-962:69409] *** End of error message ***
</pre>
{% endraw %}

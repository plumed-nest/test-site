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
[fv-az1113-981:45249] *** Process received signal ***
[fv-az1113-981:45249] Signal: Aborted (6)
[fv-az1113-981:45249] Signal code:  (-6)
[fv-az1113-981:45249] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc507242520]
[fv-az1113-981:45249] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc5072969fc]
[fv-az1113-981:45249] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc507242476]
[fv-az1113-981:45249] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc5072287f3]
[fv-az1113-981:45249] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc5076a2b9e]
[fv-az1113-981:45249] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc5076ae20c]
[fv-az1113-981:45249] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc5076ae277]
[fv-az1113-981:45249] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc5076ae52b]
[fv-az1113-981:45249] [ 8] plumed_master(+0x14274)[0x557e24085274]
[fv-az1113-981:45249] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc507229d90]
[fv-az1113-981:45249] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc507229e40]
[fv-az1113-981:45249] [11] plumed_master(+0x14ed5)[0x557e24085ed5]
[fv-az1113-981:45249] *** End of error message ***
</pre>
{% endraw %}

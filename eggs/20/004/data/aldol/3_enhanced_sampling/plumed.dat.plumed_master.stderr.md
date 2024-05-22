**Project ID:** [plumID:20.004]({{ '/' | absolute_url }}eggs/20/004/)  
Stderr for source:  aldol/3_enhanced_sampling/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Contacts.jn1okV.cpp: In constructor ‘PLMD::colvar::Contacts::Contacts(const PLMD::ActionOptions&)’:
Contacts.jn1okV.cpp:93:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
93 |   for(unsigned int i=0; i<num_atomsa; i++)
|                         ~^~~~~~~~~~~
Contacts.jn1okV.cpp:99:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
99 |   for(unsigned int i=0; i<num_atomsb; i++)
|                         ~^~~~~~~~~~~
Contacts.jn1okV.cpp:124:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
124 |   for(unsigned int i=0;i<num_atomsa;++i){
|                        ~^~~~~~~~~~~
Contacts.jn1okV.cpp:129:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
129 |   for(unsigned int i=0;i<num_atomsb;++i){
|                        ~^~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:211) void PLMD::Keywords::addFlag(const string&, bool, const string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[fv-az1113-981:44922] *** Process received signal ***
[fv-az1113-981:44922] Signal: Aborted (6)
[fv-az1113-981:44922] Signal code:  (-6)
[fv-az1113-981:44922] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ffa44042520]
[fv-az1113-981:44922] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ffa440969fc]
[fv-az1113-981:44922] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ffa44042476]
[fv-az1113-981:44922] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ffa440287f3]
[fv-az1113-981:44922] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7ffa444a2b9e]
[fv-az1113-981:44922] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7ffa444ae20c]
[fv-az1113-981:44922] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7ffa444ae277]
[fv-az1113-981:44922] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ffa444ae52b]
[fv-az1113-981:44922] [ 8] plumed_master(+0x14274)[0x55b9bb361274]
[fv-az1113-981:44922] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ffa44029d90]
[fv-az1113-981:44922] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ffa44029e40]
[fv-az1113-981:44922] [11] plumed_master(+0x14ed5)[0x55b9bb361ed5]
[fv-az1113-981:44922] *** End of error message ***
</pre>
{% endraw %}

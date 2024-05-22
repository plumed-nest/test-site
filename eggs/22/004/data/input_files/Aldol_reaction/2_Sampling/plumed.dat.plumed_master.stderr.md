**Project ID:** [plumID:22.004]({{ '/' | absolute_url }}eggs/22/004/)  
Stderr for source:  input_files/Aldol_reaction/2_Sampling/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Contacts.U2bj9E.cpp: In constructor ‘PLMD::colvar::Contacts::Contacts(const PLMD::ActionOptions&)’:
Contacts.U2bj9E.cpp:93:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
93 |   for(unsigned int i=0; i<num_atomsa; i++)
|                         ~^~~~~~~~~~~
Contacts.U2bj9E.cpp:99:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
99 |   for(unsigned int i=0; i<num_atomsb; i++)
|                         ~^~~~~~~~~~~
Contacts.U2bj9E.cpp:124:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
124 |   for(unsigned int i=0;i<num_atomsa;++i){
|                        ~^~~~~~~~~~~
Contacts.U2bj9E.cpp:129:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
129 |   for(unsigned int i=0;i<num_atomsb;++i){
|                        ~^~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:211) void PLMD::Keywords::addFlag(const string&, bool, const string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[fv-az1106-239:41719] *** Process received signal ***
[fv-az1106-239:41719] Signal: Aborted (6)
[fv-az1106-239:41719] Signal code:  (-6)
[fv-az1106-239:41719] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fed45442520]
[fv-az1106-239:41719] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fed454969fc]
[fv-az1106-239:41719] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fed45442476]
[fv-az1106-239:41719] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fed454287f3]
[fv-az1106-239:41719] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fed458a2b9e]
[fv-az1106-239:41719] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fed458ae20c]
[fv-az1106-239:41719] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fed458ae277]
[fv-az1106-239:41719] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fed458ae52b]
[fv-az1106-239:41719] [ 8] plumed_master(+0x14274)[0x5638af589274]
[fv-az1106-239:41719] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fed45429d90]
[fv-az1106-239:41719] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fed45429e40]
[fv-az1106-239:41719] [11] plumed_master(+0x14ed5)[0x5638af589ed5]
[fv-az1106-239:41719] *** End of error message ***
</pre>
{% endraw %}

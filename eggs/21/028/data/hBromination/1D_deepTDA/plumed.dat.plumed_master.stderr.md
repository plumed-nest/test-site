**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/1D_deepTDA/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../Contacts.fQAFdI.cpp: In constructor ‘PLMD::colvar::Contacts::Contacts(const PLMD::ActionOptions&)’:
../Contacts.fQAFdI.cpp:93:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
93 |   for(unsigned int i=0; i<num_atomsa; i++)
|                         ~^~~~~~~~~~~
../Contacts.fQAFdI.cpp:99:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
99 |   for(unsigned int i=0; i<num_atomsb; i++)
|                         ~^~~~~~~~~~~
../Contacts.fQAFdI.cpp:124:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
124 |   for(unsigned int i=0;i<num_atomsa;++i){
|                        ~^~~~~~~~~~~
../Contacts.fQAFdI.cpp:129:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
129 |   for(unsigned int i=0;i<num_atomsb;++i){
|                        ~^~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:211) void PLMD::Keywords::addFlag(const string&, bool, const string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[fv-az1106-239:42560] *** Process received signal ***
[fv-az1106-239:42560] Signal: Aborted (6)
[fv-az1106-239:42560] Signal code:  (-6)
[fv-az1106-239:42560] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f67dfc42520]
[fv-az1106-239:42560] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f67dfc969fc]
[fv-az1106-239:42560] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f67dfc42476]
[fv-az1106-239:42560] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f67dfc287f3]
[fv-az1106-239:42560] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f67e00a2b9e]
[fv-az1106-239:42560] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f67e00ae20c]
[fv-az1106-239:42560] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f67e00ae277]
[fv-az1106-239:42560] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f67e00ae52b]
[fv-az1106-239:42560] [ 8] plumed_master(+0x14274)[0x559f850fb274]
[fv-az1106-239:42560] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f67dfc29d90]
[fv-az1106-239:42560] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f67dfc29e40]
[fv-az1106-239:42560] [11] plumed_master(+0x14ed5)[0x559f850fbed5]
[fv-az1106-239:42560] *** End of error message ***
</pre>
{% endraw %}

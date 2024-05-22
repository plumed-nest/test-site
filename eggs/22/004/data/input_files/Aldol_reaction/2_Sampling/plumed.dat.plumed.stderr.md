**Project ID:** [plumID:22.004]({{ '/' | absolute_url }}eggs/22/004/)  
Stderr for source:  input_files/Aldol_reaction/2_Sampling/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Contacts.cpp: In constructor ‘PLMD::colvar::Contacts::Contacts(const PLMD::ActionOptions&)’:
Contacts.cpp:93:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
93 |   for(unsigned int i=0; i<num_atomsa; i++)
|                         ~^~~~~~~~~~~
Contacts.cpp:99:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
99 |   for(unsigned int i=0; i<num_atomsb; i++)
|                         ~^~~~~~~~~~~
Contacts.cpp:124:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
124 |   for(unsigned int i=0;i<num_atomsa;++i){
|                        ~^~~~~~~~~~~
Contacts.cpp:129:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
129 |   for(unsigned int i=0;i<num_atomsb;++i){
|                        ~^~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:210) void PLMD::Keywords::addFlag(const string&, bool, const string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[fv-az1106-239:41700] *** Process received signal ***
[fv-az1106-239:41700] Signal: Aborted (6)
[fv-az1106-239:41700] Signal code:  (-6)
[fv-az1106-239:41700] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f41db842520]
[fv-az1106-239:41700] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f41db8969fc]
[fv-az1106-239:41700] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f41db842476]
[fv-az1106-239:41700] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f41db8287f3]
[fv-az1106-239:41700] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f41dbca2b9e]
[fv-az1106-239:41700] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f41dbcae20c]
[fv-az1106-239:41700] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f41dbcae277]
[fv-az1106-239:41700] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f41dbcae52b]
[fv-az1106-239:41700] [ 8] plumed(+0x12f48)[0x564f7f5bef48]
[fv-az1106-239:41700] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f41db829d90]
[fv-az1106-239:41700] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f41db829e40]
[fv-az1106-239:41700] [11] plumed(+0x131e5)[0x564f7f5bf1e5]
[fv-az1106-239:41700] *** End of error message ***
</pre>
{% endraw %}

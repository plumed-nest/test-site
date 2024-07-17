**Project ID:** [plumID:20.004]({{ '/' | absolute_url }}eggs/20/004/)  
Stderr for source:  aldol/3_enhanced_sampling/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Contacts.JQJnbX.cpp: In constructor ‘PLMD::colvar::Contacts::Contacts(const PLMD::ActionOptions&)’:
Contacts.JQJnbX.cpp:93:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
93 |   for(unsigned int i=0; i<num_atomsa; i++)
|                         ~^~~~~~~~~~~
Contacts.JQJnbX.cpp:99:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
99 |   for(unsigned int i=0; i<num_atomsb; i++)
|                         ~^~~~~~~~~~~
Contacts.JQJnbX.cpp:124:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
124 |   for(unsigned int i=0;i<num_atomsa;++i){
|                        ~^~~~~~~~~~~
Contacts.JQJnbX.cpp:129:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
129 |   for(unsigned int i=0;i<num_atomsb;++i){
|                        ~^~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:211) void PLMD::Keywords::addFlag(const string&, bool, const string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[fv-az695-456:75420] *** Process received signal ***
[fv-az695-456:75420] Signal: Aborted (6)
[fv-az695-456:75420] Signal code:  (-6)
[fv-az695-456:75420] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1476042520]
[fv-az695-456:75420] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f14760969fc]
[fv-az695-456:75420] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1476042476]
[fv-az695-456:75420] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f14760287f3]
[fv-az695-456:75420] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f14764a2b9e]
[fv-az695-456:75420] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f14764ae20c]
[fv-az695-456:75420] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f14764ae277]
[fv-az695-456:75420] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f14764ae52b]
[fv-az695-456:75420] [ 8] plumed_master(+0x14274)[0x564497d76274]
[fv-az695-456:75420] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1476029d90]
[fv-az695-456:75420] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1476029e40]
[fv-az695-456:75420] [11] plumed_master(+0x14ed5)[0x564497d76ed5]
[fv-az695-456:75420] *** End of error message ***
</pre>
{% endraw %}

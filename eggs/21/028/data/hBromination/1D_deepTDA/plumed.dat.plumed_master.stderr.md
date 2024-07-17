**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/1D_deepTDA/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../Contacts.VSQ9fZ.cpp: In constructor ‘PLMD::colvar::Contacts::Contacts(const PLMD::ActionOptions&)’:
../Contacts.VSQ9fZ.cpp:93:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
93 |   for(unsigned int i=0; i<num_atomsa; i++)
|                         ~^~~~~~~~~~~
../Contacts.VSQ9fZ.cpp:99:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
99 |   for(unsigned int i=0; i<num_atomsb; i++)
|                         ~^~~~~~~~~~~
../Contacts.VSQ9fZ.cpp:124:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
124 |   for(unsigned int i=0;i<num_atomsa;++i){
|                        ~^~~~~~~~~~~
../Contacts.VSQ9fZ.cpp:129:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
129 |   for(unsigned int i=0;i<num_atomsb;++i){
|                        ~^~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:211) void PLMD::Keywords::addFlag(const string&, bool, const string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[fv-az774-16:73007] *** Process received signal ***
[fv-az774-16:73007] Signal: Aborted (6)
[fv-az774-16:73007] Signal code:  (-6)
[fv-az774-16:73007] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd63f442520]
[fv-az774-16:73007] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd63f4969fc]
[fv-az774-16:73007] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd63f442476]
[fv-az774-16:73007] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd63f4287f3]
[fv-az774-16:73007] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd63f8a2b9e]
[fv-az774-16:73007] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd63f8ae20c]
[fv-az774-16:73007] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd63f8ae277]
[fv-az774-16:73007] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd63f8ae52b]
[fv-az774-16:73007] [ 8] plumed_master(+0x14274)[0x562b587f4274]
[fv-az774-16:73007] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd63f429d90]
[fv-az774-16:73007] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd63f429e40]
[fv-az774-16:73007] [11] plumed_master(+0x14ed5)[0x562b587f4ed5]
[fv-az774-16:73007] *** End of error message ***
</pre>
{% endraw %}

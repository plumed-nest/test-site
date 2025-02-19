**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/1D_deepTDA/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../Contacts.wQC7dz.cpp: In constructor ‘PLMD::colvar::Contacts::Contacts(const PLMD::ActionOptions&)’:
../Contacts.wQC7dz.cpp:93:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
93 |   for(unsigned int i=0; i<num_atomsa; i++)
|                         ~^~~~~~~~~~~
../Contacts.wQC7dz.cpp:99:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
99 |   for(unsigned int i=0; i<num_atomsb; i++)
|                         ~^~~~~~~~~~~
../Contacts.wQC7dz.cpp:124:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
124 |   for(unsigned int i=0;i<num_atomsa;++i){
|                        ~^~~~~~~~~~~
../Contacts.wQC7dz.cpp:129:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
129 |   for(unsigned int i=0;i<num_atomsb;++i){
|                        ~^~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:263) void PLMD::Keywords::addFlag(const std::string&, bool, const std::string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[fv-az1326-415:11667] *** Process received signal ***
[fv-az1326-415:11667] Signal: Aborted (6)
[fv-az1326-415:11667] Signal code:  (-6)
[fv-az1326-415:11667] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f98c9245330]
[fv-az1326-415:11667] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f98c929eb2c]
[fv-az1326-415:11667] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f98c924527e]
[fv-az1326-415:11667] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f98c92288ff]
[fv-az1326-415:11667] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f98c96a5ff5]
[fv-az1326-415:11667] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f98c96bb0da]
[fv-az1326-415:11667] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f98c96a5a55]
[fv-az1326-415:11667] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f98c96a5a6f]
[fv-az1326-415:11667] [ 8] plumed(+0x146dd)[0x562979b886dd]
[fv-az1326-415:11667] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f98c922a1ca]
[fv-az1326-415:11667] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f98c922a28b]
[fv-az1326-415:11667] [11] plumed(+0x15365)[0x562979b89365]
[fv-az1326-415:11667] *** End of error message ***
</pre>
{% endraw %}

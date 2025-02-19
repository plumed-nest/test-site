**Project ID:** [plumID:22.004]({{ '/' | absolute_url }}eggs/22/004/)  
Stderr for source:  input_files/Aldol_reaction/2_Sampling/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Contacts.02isZc.cpp: In constructor ‘PLMD::colvar::Contacts::Contacts(const PLMD::ActionOptions&)’:
Contacts.02isZc.cpp:93:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
93 |   for(unsigned int i=0; i<num_atomsa; i++)
|                         ~^~~~~~~~~~~
Contacts.02isZc.cpp:99:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
99 |   for(unsigned int i=0; i<num_atomsb; i++)
|                         ~^~~~~~~~~~~
Contacts.02isZc.cpp:124:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
124 |   for(unsigned int i=0;i<num_atomsa;++i){
|                        ~^~~~~~~~~~~
Contacts.02isZc.cpp:129:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
129 |   for(unsigned int i=0;i<num_atomsb;++i){
|                        ~^~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:263) void PLMD::Keywords::addFlag(const std::string&, bool, const std::string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[fv-az1326-415:10899] *** Process received signal ***
[fv-az1326-415:10899] Signal: Aborted (6)
[fv-az1326-415:10899] Signal code:  (-6)
[fv-az1326-415:10899] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7ff69b045330]
[fv-az1326-415:10899] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7ff69b09eb2c]
[fv-az1326-415:10899] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7ff69b04527e]
[fv-az1326-415:10899] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7ff69b0288ff]
[fv-az1326-415:10899] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7ff69b4a5ff5]
[fv-az1326-415:10899] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7ff69b4bb0da]
[fv-az1326-415:10899] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7ff69b4a5a55]
[fv-az1326-415:10899] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7ff69b4a5a6f]
[fv-az1326-415:10899] [ 8] plumed(+0x146dd)[0x564d399c06dd]
[fv-az1326-415:10899] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7ff69b02a1ca]
[fv-az1326-415:10899] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7ff69b02a28b]
[fv-az1326-415:10899] [11] plumed(+0x15365)[0x564d399c1365]
[fv-az1326-415:10899] *** End of error message ***
</pre>
{% endraw %}

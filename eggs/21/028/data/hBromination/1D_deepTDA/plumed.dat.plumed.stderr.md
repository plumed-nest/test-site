**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/1D_deepTDA/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../Contacts.sKsj5W.cpp: In constructor ‘PLMD::colvar::Contacts::Contacts(const PLMD::ActionOptions&)’:
../Contacts.sKsj5W.cpp:93:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
93 |   for(unsigned int i=0; i<num_atomsa; i++)
|                         ~^~~~~~~~~~~
../Contacts.sKsj5W.cpp:99:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
99 |   for(unsigned int i=0; i<num_atomsb; i++)
|                         ~^~~~~~~~~~~
../Contacts.sKsj5W.cpp:124:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
124 |   for(unsigned int i=0;i<num_atomsa;++i){
|                        ~^~~~~~~~~~~
../Contacts.sKsj5W.cpp:129:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
129 |   for(unsigned int i=0;i<num_atomsb;++i){
|                        ~^~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:263) void PLMD::Keywords::addFlag(const std::string&, bool, const std::string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[runnervm1li68:10422] *** Process received signal ***
[runnervm1li68:10422] Signal: Aborted (6)
[runnervm1li68:10422] Signal code:  (-6)
[runnervm1li68:10422] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f05a6c45330]
[runnervm1li68:10422] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f05a6c9eb2c]
[runnervm1li68:10422] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f05a6c4527e]
[runnervm1li68:10422] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f05a6c288ff]
[runnervm1li68:10422] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f05a70a5ff5]
[runnervm1li68:10422] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f05a70bb0da]
[runnervm1li68:10422] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f05a70a5a55]
[runnervm1li68:10422] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f05a70a5a6f]
[runnervm1li68:10422] [ 8] plumed(+0x146dd)[0x5588f0ae06dd]
[runnervm1li68:10422] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f05a6c2a1ca]
[runnervm1li68:10422] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f05a6c2a28b]
[runnervm1li68:10422] [11] plumed(+0x15365)[0x5588f0ae1365]
[runnervm1li68:10422] *** End of error message ***
</pre>
{% endraw %}

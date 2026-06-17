**Project ID:** [plumID:20.004]({{ '/' | absolute_url }}eggs/20/004/)  
Stderr for source:  aldol/3_enhanced_sampling/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Contacts.JbQ9V7.cpp: In constructor ‘PLMD::colvar::Contacts::Contacts(const PLMD::ActionOptions&)’:
Contacts.JbQ9V7.cpp:93:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
93 |   for(unsigned int i=0; i<num_atomsa; i++)
|                         ~^~~~~~~~~~~
Contacts.JbQ9V7.cpp:99:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
99 |   for(unsigned int i=0; i<num_atomsb; i++)
|                         ~^~~~~~~~~~~
Contacts.JbQ9V7.cpp:124:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
124 |   for(unsigned int i=0;i<num_atomsa;++i){
|                        ~^~~~~~~~~~~
Contacts.JbQ9V7.cpp:129:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
129 |   for(unsigned int i=0;i<num_atomsb;++i){
|                        ~^~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:263) void PLMD::Keywords::addFlag(const std::string&, bool, const std::string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[runnervm1li68:10492] *** Process received signal ***
[runnervm1li68:10492] Signal: Aborted (6)
[runnervm1li68:10492] Signal code:  (-6)
[runnervm1li68:10492] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f91f0645330]
[runnervm1li68:10492] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f91f069eb2c]
[runnervm1li68:10492] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f91f064527e]
[runnervm1li68:10492] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f91f06288ff]
[runnervm1li68:10492] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f91f0aa5ff5]
[runnervm1li68:10492] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f91f0abb0da]
[runnervm1li68:10492] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f91f0aa5a55]
[runnervm1li68:10492] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f91f0aa5a6f]
[runnervm1li68:10492] [ 8] plumed(+0x146dd)[0x557b0a9ca6dd]
[runnervm1li68:10492] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f91f062a1ca]
[runnervm1li68:10492] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f91f062a28b]
[runnervm1li68:10492] [11] plumed(+0x15365)[0x557b0a9cb365]
[runnervm1li68:10492] *** End of error message ***
</pre>
{% endraw %}

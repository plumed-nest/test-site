**Project ID:** [plumID:22.004]({{ '/' | absolute_url }}eggs/22/004/)  
Stderr for source:  input_files/Aldol_reaction/2_Sampling/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Contacts.YZvIpK.cpp: In constructor ‘PLMD::colvar::Contacts::Contacts(const PLMD::ActionOptions&)’:
Contacts.YZvIpK.cpp:93:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
93 |   for(unsigned int i=0; i<num_atomsa; i++)
|                         ~^~~~~~~~~~~
Contacts.YZvIpK.cpp:99:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
99 |   for(unsigned int i=0; i<num_atomsb; i++)
|                         ~^~~~~~~~~~~
Contacts.YZvIpK.cpp:124:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
124 |   for(unsigned int i=0;i<num_atomsa;++i){
|                        ~^~~~~~~~~~~
Contacts.YZvIpK.cpp:129:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
129 |   for(unsigned int i=0;i<num_atomsb;++i){
|                        ~^~~~~~~~~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:211) void PLMD::Keywords::addFlag(const string&, bool, const string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[fv-az975-63:72268] *** Process received signal ***
[fv-az975-63:72268] Signal: Aborted (6)
[fv-az975-63:72268] Signal code:  (-6)
[fv-az975-63:72268] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc744c42520]
[fv-az975-63:72268] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc744c969fc]
[fv-az975-63:72268] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc744c42476]
[fv-az975-63:72268] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc744c287f3]
[fv-az975-63:72268] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc7450a2b9e]
[fv-az975-63:72268] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc7450ae20c]
[fv-az975-63:72268] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc7450ae277]
[fv-az975-63:72268] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc7450ae52b]
[fv-az975-63:72268] [ 8] plumed_master(+0x14274)[0x563780546274]
[fv-az975-63:72268] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc744c29d90]
[fv-az975-63:72268] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc744c29e40]
[fv-az975-63:72268] [11] plumed_master(+0x14ed5)[0x563780546ed5]
[fv-az975-63:72268] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Na/01_Distributions/Solid/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../../RefCV.nYqdDh.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10b' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../../../RefCV.2.10b.so ../../../RefCV.cpp

[fv-az1770-999:10423] *** Process received signal ***
[fv-az1770-999:10423] Signal: Aborted (6)
[fv-az1770-999:10423] Signal code:  (-6)
[fv-az1770-999:10423] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fced5245330]
[fv-az1770-999:10423] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fced529eb2c]
[fv-az1770-999:10423] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fced524527e]
[fv-az1770-999:10423] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fced52288ff]
[fv-az1770-999:10423] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fced56a5ff5]
[fv-az1770-999:10423] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fced56bb0da]
[fv-az1770-999:10423] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fced56a5a55]
[fv-az1770-999:10423] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fced56a5a6f]
[fv-az1770-999:10423] [ 8] plumed(+0x146dd)[0x561144f956dd]
[fv-az1770-999:10423] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fced522a1ca]
[fv-az1770-999:10423] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fced522a28b]
[fv-az1770-999:10423] [11] plumed(+0x15365)[0x561144f96365]
[fv-az1770-999:10423] *** End of error message ***
</pre>
{% endraw %}

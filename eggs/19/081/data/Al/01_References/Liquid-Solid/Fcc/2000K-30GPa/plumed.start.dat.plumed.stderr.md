**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Al/01_References/Liquid-Solid/Fcc/2000K-30GPa/plumed.start.dat   
Download: [zipped raw stdout](plumed.start.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../../../../RefCV.mpif6M.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10b' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../../../../../RefCV.2.10b.so ../../../../../RefCV.cpp

[fv-az1770-999:09911] *** Process received signal ***
[fv-az1770-999:09911] Signal: Aborted (6)
[fv-az1770-999:09911] Signal code:  (-6)
[fv-az1770-999:09911] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f934e245330]
[fv-az1770-999:09911] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f934e29eb2c]
[fv-az1770-999:09911] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f934e24527e]
[fv-az1770-999:09911] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f934e2288ff]
[fv-az1770-999:09911] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f934e6a5ff5]
[fv-az1770-999:09911] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f934e6bb0da]
[fv-az1770-999:09911] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f934e6a5a55]
[fv-az1770-999:09911] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f934e6a5a6f]
[fv-az1770-999:09911] [ 8] plumed(+0x146dd)[0x563022a266dd]
[fv-az1770-999:09911] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f934e22a1ca]
[fv-az1770-999:09911] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f934e22a28b]
[fv-az1770-999:09911] [11] plumed(+0x15365)[0x563022a27365]
[fv-az1770-999:09911] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Al/01_References/Liquid-Solid/Fcc/2000K-30GPa/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../../../../RefCV.H5aDXn.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10b' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../../../../../RefCV.2.10b.so ../../../../../RefCV.cpp

[fv-az1770-999:09824] *** Process received signal ***
[fv-az1770-999:09824] Signal: Aborted (6)
[fv-az1770-999:09824] Signal code:  (-6)
[fv-az1770-999:09824] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7ff3b8845330]
[fv-az1770-999:09824] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7ff3b889eb2c]
[fv-az1770-999:09824] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7ff3b884527e]
[fv-az1770-999:09824] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7ff3b88288ff]
[fv-az1770-999:09824] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7ff3b8ca5ff5]
[fv-az1770-999:09824] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7ff3b8cbb0da]
[fv-az1770-999:09824] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7ff3b8ca5a55]
[fv-az1770-999:09824] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7ff3b8ca5a6f]
[fv-az1770-999:09824] [ 8] plumed(+0x146dd)[0x562fe1efc6dd]
[fv-az1770-999:09824] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7ff3b882a1ca]
[fv-az1770-999:09824] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7ff3b882a28b]
[fv-az1770-999:09824] [11] plumed(+0x15365)[0x562fe1efd365]
[fv-az1770-999:09824] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Al/01_References/Liquid-Solid/Fcc/2000K-30GPa/plumed.start.dat   
Download: [zipped raw stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../../../../RefCV.iaItZv.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../../../../RefCV.2.11.0-dev.so ../../../../../RefCV.cpp

[fv-az1770-999:09944] *** Process received signal ***
[fv-az1770-999:09944] Signal: Aborted (6)
[fv-az1770-999:09944] Signal code:  (-6)
[fv-az1770-999:09944] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fac5bc45330]
[fv-az1770-999:09944] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fac5bc9eb2c]
[fv-az1770-999:09944] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fac5bc4527e]
[fv-az1770-999:09944] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fac5bc288ff]
[fv-az1770-999:09944] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fac5c0a5ff5]
[fv-az1770-999:09944] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fac5c0bb0da]
[fv-az1770-999:09944] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fac5c0a5a55]
[fv-az1770-999:09944] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fac5c0a5a6f]
[fv-az1770-999:09944] [ 8] plumed_master(+0x146dd)[0x55a333e986dd]
[fv-az1770-999:09944] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fac5bc2a1ca]
[fv-az1770-999:09944] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fac5bc2a28b]
[fv-az1770-999:09944] [11] plumed_master(+0x15365)[0x55a333e99365]
[fv-az1770-999:09944] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Al/01_References/Liquid-Solid/Bcc/2000K-30GPa/plumed.start.dat   
Download: [zipped raw stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../../../../RefCV.YXGPXp.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../../../../RefCV.2.11.0-dev.so ../../../../../RefCV.cpp

[fv-az1770-999:09771] *** Process received signal ***
[fv-az1770-999:09771] Signal: Aborted (6)
[fv-az1770-999:09771] Signal code:  (-6)
[fv-az1770-999:09771] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fc7da845330]
[fv-az1770-999:09771] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fc7da89eb2c]
[fv-az1770-999:09771] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fc7da84527e]
[fv-az1770-999:09771] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fc7da8288ff]
[fv-az1770-999:09771] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fc7daca5ff5]
[fv-az1770-999:09771] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fc7dacbb0da]
[fv-az1770-999:09771] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fc7daca5a55]
[fv-az1770-999:09771] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fc7daca5a6f]
[fv-az1770-999:09771] [ 8] plumed_master(+0x146dd)[0x557b65b3d6dd]
[fv-az1770-999:09771] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fc7da82a1ca]
[fv-az1770-999:09771] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fc7da82a28b]
[fv-az1770-999:09771] [11] plumed_master(+0x15365)[0x557b65b3e365]
[fv-az1770-999:09771] *** End of error message ***
</pre>
{% endraw %}

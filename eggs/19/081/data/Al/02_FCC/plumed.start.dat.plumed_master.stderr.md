**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Al/02_FCC/plumed.start.dat   
Download: [zipped raw stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../RefCV.VV8ZZh.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../RefCV.2.11.0-dev.so ../../RefCV.cpp

[fv-az1770-999:10115] *** Process received signal ***
[fv-az1770-999:10115] Signal: Aborted (6)
[fv-az1770-999:10115] Signal code:  (-6)
[fv-az1770-999:10115] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f85d0c45330]
[fv-az1770-999:10115] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f85d0c9eb2c]
[fv-az1770-999:10115] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f85d0c4527e]
[fv-az1770-999:10115] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f85d0c288ff]
[fv-az1770-999:10115] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f85d10a5ff5]
[fv-az1770-999:10115] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f85d10bb0da]
[fv-az1770-999:10115] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f85d10a5a55]
[fv-az1770-999:10115] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f85d10a5a6f]
[fv-az1770-999:10115] [ 8] plumed_master(+0x146dd)[0x5615df3466dd]
[fv-az1770-999:10115] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f85d0c2a1ca]
[fv-az1770-999:10115] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f85d0c2a28b]
[fv-az1770-999:10115] [11] plumed_master(+0x15365)[0x5615df347365]
[fv-az1770-999:10115] *** End of error message ***
</pre>
{% endraw %}

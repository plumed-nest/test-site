**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Al/03_BCC/plumed.start.dat   
Download: [zipped raw stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../RefCV.eKAZDG.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../RefCV.2.11.0-dev.so ../../RefCV.cpp

[fv-az1770-999:10285] *** Process received signal ***
[fv-az1770-999:10285] Signal: Aborted (6)
[fv-az1770-999:10285] Signal code:  (-6)
[fv-az1770-999:10285] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9106845330]
[fv-az1770-999:10285] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f910689eb2c]
[fv-az1770-999:10285] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f910684527e]
[fv-az1770-999:10285] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f91068288ff]
[fv-az1770-999:10285] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9106ca5ff5]
[fv-az1770-999:10285] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9106cbb0da]
[fv-az1770-999:10285] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9106ca5a55]
[fv-az1770-999:10285] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9106ca5a6f]
[fv-az1770-999:10285] [ 8] plumed_master(+0x146dd)[0x557c8cde36dd]
[fv-az1770-999:10285] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f910682a1ca]
[fv-az1770-999:10285] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f910682a28b]
[fv-az1770-999:10285] [11] plumed_master(+0x15365)[0x557c8cde4365]
[fv-az1770-999:10285] *** End of error message ***
</pre>
{% endraw %}

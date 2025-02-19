**Project ID:** [plumID:20.003]({{ '/' | absolute_url }}eggs/20/003/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
TD_TS-target-plumed2.6.Hl7Bjw.cpp:23:10: fatal error: TargetDistribution.h: No such file or directory
23 | #include "TargetDistribution.h"
|          ^~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1499) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10b' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./TD_TS-target-plumed2.6.2.10b.so TD_TS-target-plumed2.6.cpp

[fv-az1945-156:13700] *** Process received signal ***
[fv-az1945-156:13700] Signal: Aborted (6)
[fv-az1945-156:13700] Signal code:  (-6)
[fv-az1945-156:13700] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f13a7045330]
[fv-az1945-156:13700] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f13a709eb2c]
[fv-az1945-156:13700] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f13a704527e]
[fv-az1945-156:13700] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f13a70288ff]
[fv-az1945-156:13700] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f13a74a5ff5]
[fv-az1945-156:13700] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f13a74bb0da]
[fv-az1945-156:13700] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f13a74a5a55]
[fv-az1945-156:13700] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f13a74a5a6f]
[fv-az1945-156:13700] [ 8] plumed(+0x146dd)[0x5602f09716dd]
[fv-az1945-156:13700] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f13a702a1ca]
[fv-az1945-156:13700] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f13a702a28b]
[fv-az1945-156:13700] [11] plumed(+0x15365)[0x5602f0972365]
[fv-az1945-156:13700] *** End of error message ***
</pre>
{% endraw %}

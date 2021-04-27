**Project ID:** [plumID:20.003]({{ '/' | absolute_url }}eggs/20/003/)  
Stderr for source:  plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
TD_TS-target-plumed2.6.cpp:23:10: fatal error: TargetDistribution.h: No such file or directory
   23 | #include "TargetDistribution.h"
      |          ^~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:940, function void PLMD::PlumedMain::load(const string&)
+++ message follows +++
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh TD_TS-target-plumed2.6.cpp

[fv-az99-305:24679] *** Process received signal ***
[fv-az99-305:24679] Signal: Aborted (6)
[fv-az99-305:24679] Signal code:  (-6)
[fv-az99-305:24679] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fef9665c210]
[fv-az99-305:24679] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fef9665c18b]
[fv-az99-305:24679] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fef9663b859]
[fv-az99-305:24679] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fef968c3951]
[fv-az99-305:24679] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fef968cf47c]
[fv-az99-305:24679] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fef968cf4e7]
[fv-az99-305:24679] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fef968cf7ed]
[fv-az99-305:24679] [ 7] plumed_master(+0xf568)[0x559c4f190568]
[fv-az99-305:24679] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fef9663d0b3]
[fv-az99-305:24679] [ 9] plumed_master(+0xf79e)[0x559c4f19079e]
[fv-az99-305:24679] *** End of error message ***
</pre>
{% endraw %}

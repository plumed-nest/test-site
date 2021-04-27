**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
Stderr for source:  OAMe_G4/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
../code/PytorchModel.cpp:22:10: fatal error: Function.h: No such file or directory
   22 | #include "Function.h"
      |          ^~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:940, function void PLMD::PlumedMain::load(const string&)
+++ message follows +++
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../code/PytorchModel.cpp

[fv-az99-305:21991] *** Process received signal ***
[fv-az99-305:21991] Signal: Aborted (6)
[fv-az99-305:21991] Signal code:  (-6)
[fv-az99-305:21991] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f2f13faa210]
[fv-az99-305:21991] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f2f13faa18b]
[fv-az99-305:21991] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f2f13f89859]
[fv-az99-305:21991] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f2f14211951]
[fv-az99-305:21991] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f2f1421d47c]
[fv-az99-305:21991] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f2f1421d4e7]
[fv-az99-305:21991] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f2f1421d7ed]
[fv-az99-305:21991] [ 7] plumed_master(+0xf568)[0x5647f2ac8568]
[fv-az99-305:21991] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f2f13f8b0b3]
[fv-az99-305:21991] [ 9] plumed_master(+0xf79e)[0x5647f2ac879e]
[fv-az99-305:21991] *** End of error message ***
</pre>
{% endraw %}

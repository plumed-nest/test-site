**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
Stderr for source:  OAMe_G1/plumed.dat   
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

[fv-az99-305:21882] *** Process received signal ***
[fv-az99-305:21882] Signal: Aborted (6)
[fv-az99-305:21882] Signal code:  (-6)
[fv-az99-305:21882] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa64a9da210]
[fv-az99-305:21882] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa64a9da18b]
[fv-az99-305:21882] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa64a9b9859]
[fv-az99-305:21882] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa64ac41951]
[fv-az99-305:21882] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa64ac4d47c]
[fv-az99-305:21882] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa64ac4d4e7]
[fv-az99-305:21882] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fa64ac4d7ed]
[fv-az99-305:21882] [ 7] plumed_master(+0xf568)[0x558eebfb1568]
[fv-az99-305:21882] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa64a9bb0b3]
[fv-az99-305:21882] [ 9] plumed_master(+0xf79e)[0x558eebfb179e]
[fv-az99-305:21882] *** End of error message ***
</pre>
{% endraw %}

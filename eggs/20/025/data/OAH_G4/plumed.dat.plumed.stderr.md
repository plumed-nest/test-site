**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
Stderr for source:  OAH_G4/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
../code/PytorchModel.cpp:22:10: fatal error: Function.h: No such file or directory
   22 | #include "Function.h"
      |          ^~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:942, function void PLMD::PlumedMain::load(const string&)
+++ message follows +++
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed"/scripts/mklib.sh ../code/PytorchModel.cpp

[fv-az99-305:21721] *** Process received signal ***
[fv-az99-305:21721] Signal: Aborted (6)
[fv-az99-305:21721] Signal code:  (-6)
[fv-az99-305:21721] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f841bfdc210]
[fv-az99-305:21721] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f841bfdc18b]
[fv-az99-305:21721] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f841bfbb859]
[fv-az99-305:21721] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f841c243951]
[fv-az99-305:21721] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f841c24f47c]
[fv-az99-305:21721] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f841c24f4e7]
[fv-az99-305:21721] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f841c24f799]
[fv-az99-305:21721] [ 7] plumed(+0xf47d)[0x5646391ec47d]
[fv-az99-305:21721] [ 8] plumed(+0x14004)[0x5646391f1004]
[fv-az99-305:21721] [ 9] plumed(+0xf698)[0x5646391ec698]
[fv-az99-305:21721] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f841bfbd0b3]
[fv-az99-305:21721] [11] plumed(+0xf76e)[0x5646391ec76e]
[fv-az99-305:21721] *** End of error message ***
</pre>
{% endraw %}

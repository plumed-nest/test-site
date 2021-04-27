**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
Stderr for source:  OAH_G6/plumed.dat   
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

[fv-az99-305:21795] *** Process received signal ***
[fv-az99-305:21795] Signal: Aborted (6)
[fv-az99-305:21795] Signal code:  (-6)
[fv-az99-305:21795] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f536b0f2210]
[fv-az99-305:21795] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f536b0f218b]
[fv-az99-305:21795] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f536b0d1859]
[fv-az99-305:21795] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f536b359951]
[fv-az99-305:21795] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f536b36547c]
[fv-az99-305:21795] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f536b3654e7]
[fv-az99-305:21795] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f536b365799]
[fv-az99-305:21795] [ 7] plumed(+0xf47d)[0x55ca298d147d]
[fv-az99-305:21795] [ 8] plumed(+0x14004)[0x55ca298d6004]
[fv-az99-305:21795] [ 9] plumed(+0xf698)[0x55ca298d1698]
[fv-az99-305:21795] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f536b0d30b3]
[fv-az99-305:21795] [11] plumed(+0xf76e)[0x55ca298d176e]
[fv-az99-305:21795] *** End of error message ***
</pre>
{% endraw %}

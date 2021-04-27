**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
Stderr for source:  OAMe_G2/plumed.dat   
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

[fv-az99-305:21904] *** Process received signal ***
[fv-az99-305:21904] Signal: Aborted (6)
[fv-az99-305:21904] Signal code:  (-6)
[fv-az99-305:21904] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa139a7a210]
[fv-az99-305:21904] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa139a7a18b]
[fv-az99-305:21904] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa139a59859]
[fv-az99-305:21904] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa139ce1951]
[fv-az99-305:21904] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa139ced47c]
[fv-az99-305:21904] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa139ced4e7]
[fv-az99-305:21904] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fa139ced799]
[fv-az99-305:21904] [ 7] plumed(+0xf47d)[0x55dd94e5e47d]
[fv-az99-305:21904] [ 8] plumed(+0x14004)[0x55dd94e63004]
[fv-az99-305:21904] [ 9] plumed(+0xf698)[0x55dd94e5e698]
[fv-az99-305:21904] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa139a5b0b3]
[fv-az99-305:21904] [11] plumed(+0xf76e)[0x55dd94e5e76e]
[fv-az99-305:21904] *** End of error message ***
</pre>
{% endraw %}

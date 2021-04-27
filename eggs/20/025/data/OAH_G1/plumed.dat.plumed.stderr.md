**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
Stderr for source:  OAH_G1/plumed.dat   
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

[fv-az99-305:21612] *** Process received signal ***
[fv-az99-305:21612] Signal: Aborted (6)
[fv-az99-305:21612] Signal code:  (-6)
[fv-az99-305:21612] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f1a0b2f6210]
[fv-az99-305:21612] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f1a0b2f618b]
[fv-az99-305:21612] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f1a0b2d5859]
[fv-az99-305:21612] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f1a0b55d951]
[fv-az99-305:21612] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f1a0b56947c]
[fv-az99-305:21612] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f1a0b5694e7]
[fv-az99-305:21612] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f1a0b569799]
[fv-az99-305:21612] [ 7] plumed(+0xf47d)[0x55bbce3f747d]
[fv-az99-305:21612] [ 8] plumed(+0x14004)[0x55bbce3fc004]
[fv-az99-305:21612] [ 9] plumed(+0xf698)[0x55bbce3f7698]
[fv-az99-305:21612] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f1a0b2d70b3]
[fv-az99-305:21612] [11] plumed(+0xf76e)[0x55bbce3f776e]
[fv-az99-305:21612] *** End of error message ***
</pre>
{% endraw %}

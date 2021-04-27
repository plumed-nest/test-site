**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
Stderr for source:  OAMe_alone/plumed.dat   
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

[fv-az99-305:22085] *** Process received signal ***
[fv-az99-305:22085] Signal: Aborted (6)
[fv-az99-305:22085] Signal code:  (-6)
[fv-az99-305:22085] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4c5a33d210]
[fv-az99-305:22085] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4c5a33d18b]
[fv-az99-305:22085] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4c5a31c859]
[fv-az99-305:22085] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4c5a5a4951]
[fv-az99-305:22085] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f4c5a5b047c]
[fv-az99-305:22085] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f4c5a5b04e7]
[fv-az99-305:22085] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4c5a5b0799]
[fv-az99-305:22085] [ 7] plumed(+0xf47d)[0x55dc8e7a847d]
[fv-az99-305:22085] [ 8] plumed(+0x14004)[0x55dc8e7ad004]
[fv-az99-305:22085] [ 9] plumed(+0xf698)[0x55dc8e7a8698]
[fv-az99-305:22085] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4c5a31e0b3]
[fv-az99-305:22085] [11] plumed(+0xf76e)[0x55dc8e7a876e]
[fv-az99-305:22085] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
Stderr for source:  OAMe_G1/plumed.dat   
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

[fv-az99-305:21868] *** Process received signal ***
[fv-az99-305:21868] Signal: Aborted (6)
[fv-az99-305:21868] Signal code:  (-6)
[fv-az99-305:21868] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f702f91a210]
[fv-az99-305:21868] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f702f91a18b]
[fv-az99-305:21868] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f702f8f9859]
[fv-az99-305:21868] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f702fb81951]
[fv-az99-305:21868] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f702fb8d47c]
[fv-az99-305:21868] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f702fb8d4e7]
[fv-az99-305:21868] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f702fb8d799]
[fv-az99-305:21868] [ 7] plumed(+0xf47d)[0x5610adc8947d]
[fv-az99-305:21868] [ 8] plumed(+0x14004)[0x5610adc8e004]
[fv-az99-305:21868] [ 9] plumed(+0xf698)[0x5610adc89698]
[fv-az99-305:21868] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f702f8fb0b3]
[fv-az99-305:21868] [11] plumed(+0xf76e)[0x5610adc8976e]
[fv-az99-305:21868] *** End of error message ***
</pre>
{% endraw %}

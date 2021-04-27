**Project ID:** [plumID:20.004]({{ '/' | absolute_url }}eggs/20/004/)  
Stderr for source:  aldol/3_enhanced_sampling/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
../../code/PytorchModel.cpp:25:10: fatal error: torch/torch.h: No such file or directory
   25 | #include <torch/torch.h>
      |          ^~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:942, function void PLMD::PlumedMain::load(const string&)
+++ message follows +++
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed"/scripts/mklib.sh ../../code/PytorchModel.cpp

[fv-az99-305:24623] *** Process received signal ***
[fv-az99-305:24623] Signal: Aborted (6)
[fv-az99-305:24623] Signal code:  (-6)
[fv-az99-305:24623] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc182252210]
[fv-az99-305:24623] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc18225218b]
[fv-az99-305:24623] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc182231859]
[fv-az99-305:24623] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc1824b9951]
[fv-az99-305:24623] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc1824c547c]
[fv-az99-305:24623] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc1824c54e7]
[fv-az99-305:24623] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc1824c5799]
[fv-az99-305:24623] [ 7] plumed(+0xf47d)[0x560d5603e47d]
[fv-az99-305:24623] [ 8] plumed(+0x14004)[0x560d56043004]
[fv-az99-305:24623] [ 9] plumed(+0xf698)[0x560d5603e698]
[fv-az99-305:24623] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc1822330b3]
[fv-az99-305:24623] [11] plumed(+0xf76e)[0x560d5603e76e]
[fv-az99-305:24623] *** End of error message ***
</pre>
{% endraw %}

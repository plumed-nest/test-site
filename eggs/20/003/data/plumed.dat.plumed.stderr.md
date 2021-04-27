**Project ID:** [plumID:20.003]({{ '/' | absolute_url }}eggs/20/003/)  
Stderr for source:  plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
TD_TS-target-plumed2.6.cpp:23:10: fatal error: TargetDistribution.h: No such file or directory
   23 | #include "TargetDistribution.h"
      |          ^~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:942, function void PLMD::PlumedMain::load(const string&)
+++ message follows +++
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed"/scripts/mklib.sh TD_TS-target-plumed2.6.cpp

[fv-az99-305:24665] *** Process received signal ***
[fv-az99-305:24665] Signal: Aborted (6)
[fv-az99-305:24665] Signal code:  (-6)
[fv-az99-305:24665] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f34a555f210]
[fv-az99-305:24665] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f34a555f18b]
[fv-az99-305:24665] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f34a553e859]
[fv-az99-305:24665] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f34a57c6951]
[fv-az99-305:24665] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f34a57d247c]
[fv-az99-305:24665] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f34a57d24e7]
[fv-az99-305:24665] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f34a57d2799]
[fv-az99-305:24665] [ 7] plumed(+0xf47d)[0x561c88ea747d]
[fv-az99-305:24665] [ 8] plumed(+0x14004)[0x561c88eac004]
[fv-az99-305:24665] [ 9] plumed(+0xf698)[0x561c88ea7698]
[fv-az99-305:24665] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f34a55400b3]
[fv-az99-305:24665] [11] plumed(+0xf76e)[0x561c88ea776e]
[fv-az99-305:24665] *** End of error message ***
</pre>
{% endraw %}

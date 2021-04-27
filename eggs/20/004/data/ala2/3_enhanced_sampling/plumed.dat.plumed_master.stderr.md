**Project ID:** [plumID:20.004]({{ '/' | absolute_url }}eggs/20/004/)  
Stderr for source:  ala2/3_enhanced_sampling/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
../../code/PytorchModel.cpp:25:10: fatal error: torch/torch.h: No such file or directory
   25 | #include <torch/torch.h>
      |          ^~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:940, function void PLMD::PlumedMain::load(const string&)
+++ message follows +++
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed_master" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed_master" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed_master" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh ../../code/PytorchModel.cpp

[fv-az99-305:24601] *** Process received signal ***
[fv-az99-305:24601] Signal: Aborted (6)
[fv-az99-305:24601] Signal code:  (-6)
[fv-az99-305:24601] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9e2d7a4210]
[fv-az99-305:24601] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f9e2d7a418b]
[fv-az99-305:24601] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9e2d783859]
[fv-az99-305:24601] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f9e2da0b951]
[fv-az99-305:24601] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f9e2da1747c]
[fv-az99-305:24601] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f9e2da174e7]
[fv-az99-305:24601] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f9e2da177ed]
[fv-az99-305:24601] [ 7] plumed_master(+0xf568)[0x56518a691568]
[fv-az99-305:24601] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f9e2d7850b3]
[fv-az99-305:24601] [ 9] plumed_master(+0xf79e)[0x56518a69179e]
[fv-az99-305:24601] *** End of error message ***
</pre>
{% endraw %}

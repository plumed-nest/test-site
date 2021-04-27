**Project ID:** [plumID:20.004]({{ '/' | absolute_url }}eggs/20/004/)  
Stderr for source:  aldol/3_enhanced_sampling/plumed.dat   
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

[fv-az99-305:24638] *** Process received signal ***
[fv-az99-305:24638] Signal: Aborted (6)
[fv-az99-305:24638] Signal code:  (-6)
[fv-az99-305:24638] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb95bb76210]
[fv-az99-305:24638] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb95bb7618b]
[fv-az99-305:24638] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb95bb55859]
[fv-az99-305:24638] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb95bddd951]
[fv-az99-305:24638] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb95bde947c]
[fv-az99-305:24638] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb95bde94e7]
[fv-az99-305:24638] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fb95bde97ed]
[fv-az99-305:24638] [ 7] plumed_master(+0xf568)[0x563bae403568]
[fv-az99-305:24638] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb95bb570b3]
[fv-az99-305:24638] [ 9] plumed_master(+0xf79e)[0x563bae40379e]
[fv-az99-305:24638] *** End of error message ***
</pre>
{% endraw %}

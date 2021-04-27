**Project ID:** [plumID:19.005]({{ '/' | absolute_url }}eggs/19/005/)  
Stderr for source:  cmyc_alone/plumed/plumed_master.dat   
(download [zipped raw stdout](plumed_master.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:128, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.ha_.*)
[fv-az99-305:43950] *** Process received signal ***
[fv-az99-305:43950] Signal: Aborted (6)
[fv-az99-305:43950] Signal code:  (-6)
[fv-az99-305:43950] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f241739b210]
[fv-az99-305:43950] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f241739b18b]
[fv-az99-305:43950] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f241737a859]
[fv-az99-305:43950] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f2417602951]
[fv-az99-305:43950] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f241760e47c]
[fv-az99-305:43950] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f241760e4e7]
[fv-az99-305:43950] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f241760e7ed]
[fv-az99-305:43950] [ 7] plumed_master(+0xf568)[0x5573f81d3568]
[fv-az99-305:43950] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f241737c0b3]
[fv-az99-305:43950] [ 9] plumed_master(+0xf79e)[0x5573f81d379e]
[fv-az99-305:43950] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:128, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.ha_.*)
[fv-az99-305:43951] *** Process received signal ***
[fv-az99-305:43951] Signal: Aborted (6)
[fv-az99-305:43951] Signal code:  (-6)
[fv-az99-305:43951] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7faee0dd4210]
[fv-az99-305:43951] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7faee0dd418b]
[fv-az99-305:43951] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7faee0db3859]
[fv-az99-305:43951] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7faee103b951]
[fv-az99-305:43951] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7faee104747c]
[fv-az99-305:43951] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7faee10474e7]
[fv-az99-305:43951] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7faee10477ed]
[fv-az99-305:43951] [ 7] plumed_master(+0xf568)[0x55ecffb5e568]
[fv-az99-305:43951] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7faee0db50b3]
[fv-az99-305:43951] [ 9] plumed_master(+0xf79e)[0x55ecffb5e79e]
[fv-az99-305:43951] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

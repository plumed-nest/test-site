**Project ID:** [plumID:19.005]({{ '/' | absolute_url }}eggs/19/005/)  
Stderr for source:  cmyc_and_10058_F4/plumed/plumed_master.dat   
(download [zipped raw stdout](plumed_master.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:128, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.ha_.*)
[fv-az99-305:43985] *** Process received signal ***
[fv-az99-305:43985] Signal: Aborted (6)
[fv-az99-305:43985] Signal code:  (-6)
[fv-az99-305:43985] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f218f1ab210]
[fv-az99-305:43985] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f218f1ab18b]
[fv-az99-305:43985] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f218f18a859]
[fv-az99-305:43985] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f218f412951]
[fv-az99-305:43985] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f218f41e47c]
[fv-az99-305:43985] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f218f41e4e7]
[fv-az99-305:43985] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f218f41e7ed]
[fv-az99-305:43985] [ 7] plumed_master(+0xf568)[0x556040a00568]
[fv-az99-305:43985] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f218f18c0b3]
[fv-az99-305:43985] [ 9] plumed_master(+0xf79e)[0x556040a0079e]
[fv-az99-305:43985] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:128, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.ha_.*)
[fv-az99-305:43984] *** Process received signal ***
[fv-az99-305:43984] Signal: Aborted (6)
[fv-az99-305:43984] Signal code:  (-6)
[fv-az99-305:43984] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9916f62210]
[fv-az99-305:43984] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f9916f6218b]
[fv-az99-305:43984] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9916f41859]
[fv-az99-305:43984] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f99171c9951]
[fv-az99-305:43984] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f99171d547c]
[fv-az99-305:43984] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f99171d54e7]
[fv-az99-305:43984] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f99171d57ed]
[fv-az99-305:43984] [ 7] plumed_master(+0xf568)[0x55c7a01ca568]
[fv-az99-305:43984] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f9916f430b3]
[fv-az99-305:43984] [ 9] plumed_master(+0xf79e)[0x55c7a01ca79e]
[fv-az99-305:43984] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 1 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

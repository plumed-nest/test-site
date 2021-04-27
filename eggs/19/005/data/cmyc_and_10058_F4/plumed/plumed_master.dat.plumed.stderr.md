**Project ID:** [plumID:19.005]({{ '/' | absolute_url }}eggs/19/005/)  
Stderr for source:  cmyc_and_10058_F4/plumed/plumed_master.dat   
(download [zipped raw stdout](plumed_master.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:129, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.ha_.*)
[fv-az99-305:43970] *** Process received signal ***
[fv-az99-305:43970] Signal: Aborted (6)
[fv-az99-305:43970] Signal code:  (-6)
[fv-az99-305:43970] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fbdf8982210]
[fv-az99-305:43970] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fbdf898218b]
[fv-az99-305:43970] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fbdf8961859]
[fv-az99-305:43970] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fbdf8be9951]
[fv-az99-305:43970] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fbdf8bf547c]
[fv-az99-305:43970] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fbdf8bf54e7]
[fv-az99-305:43970] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fbdf8bf5799]
[fv-az99-305:43970] [ 7] plumed(+0xf47d)[0x55d9b55de47d]
[fv-az99-305:43970] [ 8] plumed(+0x14004)[0x55d9b55e3004]
[fv-az99-305:43970] [ 9] plumed(+0xf698)[0x55d9b55de698]
[fv-az99-305:43970] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fbdf89630b3]
[fv-az99-305:43970] [11] plumed(+0xf76e)[0x55d9b55de76e]
[fv-az99-305:43970] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:129, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.ha_.*)
[fv-az99-305:43971] *** Process received signal ***
[fv-az99-305:43971] Signal: Aborted (6)
[fv-az99-305:43971] Signal code:  (-6)
[fv-az99-305:43971] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fecdd865210]
[fv-az99-305:43971] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fecdd86518b]
[fv-az99-305:43971] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fecdd844859]
[fv-az99-305:43971] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fecddacc951]
[fv-az99-305:43971] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fecddad847c]
[fv-az99-305:43971] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fecddad84e7]
[fv-az99-305:43971] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fecddad8799]
[fv-az99-305:43971] [ 7] plumed(+0xf47d)[0x557473e3e47d]
[fv-az99-305:43971] [ 8] plumed(+0x14004)[0x557473e43004]
[fv-az99-305:43971] [ 9] plumed(+0xf698)[0x557473e3e698]
[fv-az99-305:43971] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fecdd8460b3]
[fv-az99-305:43971] [11] plumed(+0xf76e)[0x557473e3e76e]
[fv-az99-305:43971] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

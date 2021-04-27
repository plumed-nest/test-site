**Project ID:** [plumID:19.005]({{ '/' | absolute_url }}eggs/19/005/)  
Stderr for source:  cmyc_alone/plumed/plumed_master.dat   
(download [zipped raw stdout](plumed_master.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:129, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.ha_.*)
[fv-az99-305:43938] *** Process received signal ***
[fv-az99-305:43938] Signal: Aborted (6)
[fv-az99-305:43938] Signal code:  (-6)
[fv-az99-305:43938] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9247c12210]
[fv-az99-305:43938] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f9247c1218b]
[fv-az99-305:43938] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9247bf1859]
[fv-az99-305:43938] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f9247e79951]
[fv-az99-305:43938] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f9247e8547c]
[fv-az99-305:43938] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f9247e854e7]
[fv-az99-305:43938] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f9247e85799]
[fv-az99-305:43938] [ 7] plumed(+0xf47d)[0x55ad7549447d]
[fv-az99-305:43938] [ 8] plumed(+0x14004)[0x55ad75499004]
[fv-az99-305:43938] [ 9] plumed(+0xf698)[0x55ad75494698]
[fv-az99-305:43938] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f9247bf30b3]
[fv-az99-305:43938] [11] plumed(+0xf76e)[0x55ad7549476e]
[fv-az99-305:43938] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:129, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.ha_.*)
[fv-az99-305:43937] *** Process received signal ***
[fv-az99-305:43937] Signal: Aborted (6)
[fv-az99-305:43937] Signal code:  (-6)
[fv-az99-305:43937] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f86659da210]
[fv-az99-305:43937] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f86659da18b]
[fv-az99-305:43937] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f86659b9859]
[fv-az99-305:43937] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f8665c41951]
[fv-az99-305:43937] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f8665c4d47c]
[fv-az99-305:43937] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f8665c4d4e7]
[fv-az99-305:43937] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f8665c4d799]
[fv-az99-305:43937] [ 7] plumed(+0xf47d)[0x5636b403147d]
[fv-az99-305:43937] [ 8] plumed(+0x14004)[0x5636b4036004]
[fv-az99-305:43937] [ 9] plumed(+0xf698)[0x5636b4031698]
[fv-az99-305:43937] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f86659bb0b3]
[fv-az99-305:43937] [11] plumed(+0xf76e)[0x5636b403176e]
[fv-az99-305:43937] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 1 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

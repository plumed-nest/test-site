**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  Crystallization/IceIc/96molecules/Multithermal/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=330 MIN_TEMP=300 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18161] *** Process received signal ***
[fv-az99-305:18161] Signal: Aborted (6)
[fv-az99-305:18161] Signal code:  (-6)
[fv-az99-305:18161] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f8847674210]
[fv-az99-305:18161] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f884767418b]
[fv-az99-305:18161] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f8847653859]
[fv-az99-305:18161] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f88478db951]
[fv-az99-305:18161] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f88478e747c]
[fv-az99-305:18161] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f88478e74e7]
[fv-az99-305:18161] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f88478e7799]
[fv-az99-305:18161] [ 7] plumed(+0xf47d)[0x55a98f65547d]
[fv-az99-305:18161] [ 8] plumed(+0x14004)[0x55a98f65a004]
[fv-az99-305:18161] [ 9] plumed(+0xf698)[0x55a98f655698]
[fv-az99-305:18161] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f88476550b3]
[fv-az99-305:18161] [11] plumed(+0xf76e)[0x55a98f65576e]
[fv-az99-305:18161] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=330 MIN_TEMP=300 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18160] *** Process received signal ***
[fv-az99-305:18160] Signal: Aborted (6)
[fv-az99-305:18160] Signal code:  (-6)
[fv-az99-305:18160] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5f0d7bc210]
[fv-az99-305:18160] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5f0d7bc18b]
[fv-az99-305:18160] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5f0d79b859]
[fv-az99-305:18160] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5f0da23951]
[fv-az99-305:18160] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5f0da2f47c]
[fv-az99-305:18160] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5f0da2f4e7]
[fv-az99-305:18160] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f5f0da2f799]
[fv-az99-305:18160] [ 7] plumed(+0xf47d)[0x55ffaaa4747d]
[fv-az99-305:18160] [ 8] plumed(+0x14004)[0x55ffaaa4c004]
[fv-az99-305:18160] [ 9] plumed(+0xf698)[0x55ffaaa47698]
[fv-az99-305:18160] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5f0d79d0b3]
[fv-az99-305:18160] [11] plumed(+0xf76e)[0x55ffaaa4776e]
[fv-az99-305:18160] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 1 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

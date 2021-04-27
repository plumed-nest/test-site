**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  Crystallization/IceIh/96molecules/Multithermal/plumed.start.dat   
(download [zipped raw stdout](plumed.start.dat.plumed.stdout.txt.zip))  
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
[fv-az99-305:18422] *** Process received signal ***
[fv-az99-305:18422] Signal: Aborted (6)
[fv-az99-305:18422] Signal code:  (-6)
[fv-az99-305:18422] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f8e4331d210]
[fv-az99-305:18422] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f8e4331d18b]
[fv-az99-305:18422] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f8e432fc859]
[fv-az99-305:18422] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f8e43584951]
[fv-az99-305:18422] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f8e4359047c]
[fv-az99-305:18422] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f8e435904e7]
[fv-az99-305:18422] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f8e43590799]
[fv-az99-305:18422] [ 7] plumed(+0xf47d)[0x55f84766147d]
[fv-az99-305:18422] [ 8] plumed(+0x14004)[0x55f847666004]
[fv-az99-305:18422] [ 9] plumed(+0xf698)[0x55f847661698]
[fv-az99-305:18422] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f8e432fe0b3]
[fv-az99-305:18422] [11] plumed(+0xf76e)[0x55f84766176e]
[fv-az99-305:18422] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=330 MIN_TEMP=300 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18423] *** Process received signal ***
[fv-az99-305:18423] Signal: Aborted (6)
[fv-az99-305:18423] Signal code:  (-6)
[fv-az99-305:18423] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4eafda7210]
[fv-az99-305:18423] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4eafda718b]
[fv-az99-305:18423] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4eafd86859]
[fv-az99-305:18423] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4eb000e951]
[fv-az99-305:18423] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f4eb001a47c]
[fv-az99-305:18423] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f4eb001a4e7]
[fv-az99-305:18423] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4eb001a799]
[fv-az99-305:18423] [ 7] plumed(+0xf47d)[0x5630daa8e47d]
[fv-az99-305:18423] [ 8] plumed(+0x14004)[0x5630daa93004]
[fv-az99-305:18423] [ 9] plumed(+0xf698)[0x5630daa8e698]
[fv-az99-305:18423] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4eafd880b3]
[fv-az99-305:18423] [11] plumed(+0xf76e)[0x5630daa8e76e]
[fv-az99-305:18423] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  Crystallization/IceIh/96molecules/Multithermal/plumed.dat   
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
[fv-az99-305:18392] *** Process received signal ***
[fv-az99-305:18392] Signal: Aborted (6)
[fv-az99-305:18392] Signal code:  (-6)
[fv-az99-305:18392] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f641fc77210]
[fv-az99-305:18392] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f641fc7718b]
[fv-az99-305:18392] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f641fc56859]
[fv-az99-305:18392] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f641fede951]
[fv-az99-305:18392] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f641feea47c]
[fv-az99-305:18392] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f641feea4e7]
[fv-az99-305:18392] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f641feea799]
[fv-az99-305:18392] [ 7] plumed(+0xf47d)[0x561f55b1e47d]
[fv-az99-305:18392] [ 8] plumed(+0x14004)[0x561f55b23004]
[fv-az99-305:18392] [ 9] plumed(+0xf698)[0x561f55b1e698]
[fv-az99-305:18392] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f641fc580b3]
[fv-az99-305:18392] [11] plumed(+0xf76e)[0x561f55b1e76e]
[fv-az99-305:18392] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=330 MIN_TEMP=300 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18393] *** Process received signal ***
[fv-az99-305:18393] Signal: Aborted (6)
[fv-az99-305:18393] Signal code:  (-6)
[fv-az99-305:18393] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5d72348210]
[fv-az99-305:18393] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5d7234818b]
[fv-az99-305:18393] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5d72327859]
[fv-az99-305:18393] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5d725af951]
[fv-az99-305:18393] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5d725bb47c]
[fv-az99-305:18393] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5d725bb4e7]
[fv-az99-305:18393] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f5d725bb799]
[fv-az99-305:18393] [ 7] plumed(+0xf47d)[0x559b5081247d]
[fv-az99-305:18393] [ 8] plumed(+0x14004)[0x559b50817004]
[fv-az99-305:18393] [ 9] plumed(+0xf698)[0x559b50812698]
[fv-az99-305:18393] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5d723290b3]
[fv-az99-305:18393] [11] plumed(+0xf76e)[0x559b5081276e]
[fv-az99-305:18393] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  MultithermalSimulations/IceIc/64molecules/Template/plumed.start.dat   
(download [zipped raw stdout](plumed.start.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=225 MIN_TEMP=100 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18551] *** Process received signal ***
[fv-az99-305:18551] Signal: Aborted (6)
[fv-az99-305:18551] Signal code:  (-6)
[fv-az99-305:18551] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f297bd2d210]
[fv-az99-305:18551] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f297bd2d18b]
[fv-az99-305:18551] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f297bd0c859]
[fv-az99-305:18551] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f297bf94951]
[fv-az99-305:18551] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f297bfa047c]
[fv-az99-305:18551] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f297bfa04e7]
[fv-az99-305:18551] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f297bfa0799]
[fv-az99-305:18551] [ 7] plumed(+0xf47d)[0x55ec7626947d]
[fv-az99-305:18551] [ 8] plumed(+0x14004)[0x55ec7626e004]
[fv-az99-305:18551] [ 9] plumed(+0xf698)[0x55ec76269698]
[fv-az99-305:18551] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f297bd0e0b3]
[fv-az99-305:18551] [11] plumed(+0xf76e)[0x55ec7626976e]
[fv-az99-305:18551] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=225 MIN_TEMP=100 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18552] *** Process received signal ***
[fv-az99-305:18552] Signal: Aborted (6)
[fv-az99-305:18552] Signal code:  (-6)
[fv-az99-305:18552] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fec9cec2210]
[fv-az99-305:18552] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fec9cec218b]
[fv-az99-305:18552] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fec9cea1859]
[fv-az99-305:18552] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fec9d129951]
[fv-az99-305:18552] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fec9d13547c]
[fv-az99-305:18552] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fec9d1354e7]
[fv-az99-305:18552] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fec9d135799]
[fv-az99-305:18552] [ 7] plumed(+0xf47d)[0x5561a86f047d]
[fv-az99-305:18552] [ 8] plumed(+0x14004)[0x5561a86f5004]
[fv-az99-305:18552] [ 9] plumed(+0xf698)[0x5561a86f0698]
[fv-az99-305:18552] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fec9cea30b3]
[fv-az99-305:18552] [11] plumed(+0xf76e)[0x5561a86f076e]
[fv-az99-305:18552] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

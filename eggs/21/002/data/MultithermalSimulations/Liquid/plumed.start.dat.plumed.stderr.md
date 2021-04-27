**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  MultithermalSimulations/Liquid/plumed.start.dat   
(download [zipped raw stdout](plumed.start.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=350 MIN_TEMP=260 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18737] *** Process received signal ***
[fv-az99-305:18737] Signal: Aborted (6)
[fv-az99-305:18737] Signal code:  (-6)
[fv-az99-305:18737] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc65e59d210]
[fv-az99-305:18737] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc65e59d18b]
[fv-az99-305:18737] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc65e57c859]
[fv-az99-305:18737] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc65e804951]
[fv-az99-305:18737] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc65e81047c]
[fv-az99-305:18737] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc65e8104e7]
[fv-az99-305:18737] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc65e810799]
[fv-az99-305:18737] [ 7] plumed(+0xf47d)[0x5621b63f047d]
[fv-az99-305:18737] [ 8] plumed(+0x14004)[0x5621b63f5004]
[fv-az99-305:18737] [ 9] plumed(+0xf698)[0x5621b63f0698]
[fv-az99-305:18737] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc65e57e0b3]
[fv-az99-305:18737] [11] plumed(+0xf76e)[0x5621b63f076e]
[fv-az99-305:18737] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=350 MIN_TEMP=260 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18738] *** Process received signal ***
[fv-az99-305:18738] Signal: Aborted (6)
[fv-az99-305:18738] Signal code:  (-6)
[fv-az99-305:18738] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5544c83210]
[fv-az99-305:18738] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5544c8318b]
[fv-az99-305:18738] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5544c62859]
[fv-az99-305:18738] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5544eea951]
[fv-az99-305:18738] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5544ef647c]
[fv-az99-305:18738] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5544ef64e7]
[fv-az99-305:18738] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f5544ef6799]
[fv-az99-305:18738] [ 7] plumed(+0xf47d)[0x55e7f4ef647d]
[fv-az99-305:18738] [ 8] plumed(+0x14004)[0x55e7f4efb004]
[fv-az99-305:18738] [ 9] plumed(+0xf698)[0x55e7f4ef6698]
[fv-az99-305:18738] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5544c640b3]
[fv-az99-305:18738] [11] plumed(+0xf76e)[0x55e7f4ef676e]
[fv-az99-305:18738] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 1 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

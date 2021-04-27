**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  MultithermalSimulations/IceIh/288molecules/Template/plumed.start.dat   
(download [zipped raw stdout](plumed.start.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=305 MIN_TEMP=260 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18675] *** Process received signal ***
[fv-az99-305:18675] Signal: Aborted (6)
[fv-az99-305:18675] Signal code:  (-6)
[fv-az99-305:18675] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f6551edb210]
[fv-az99-305:18675] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f6551edb18b]
[fv-az99-305:18675] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f6551eba859]
[fv-az99-305:18675] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f6552142951]
[fv-az99-305:18675] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f655214e47c]
[fv-az99-305:18675] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f655214e4e7]
[fv-az99-305:18675] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f655214e799]
[fv-az99-305:18675] [ 7] plumed(+0xf47d)[0x556088bcb47d]
[fv-az99-305:18675] [ 8] plumed(+0x14004)[0x556088bd0004]
[fv-az99-305:18675] [ 9] plumed(+0xf698)[0x556088bcb698]
[fv-az99-305:18675] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f6551ebc0b3]
[fv-az99-305:18675] [11] plumed(+0xf76e)[0x556088bcb76e]
[fv-az99-305:18675] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=305 MIN_TEMP=260 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18674] *** Process received signal ***
[fv-az99-305:18674] Signal: Aborted (6)
[fv-az99-305:18674] Signal code:  (-6)
[fv-az99-305:18674] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f41a0055210]
[fv-az99-305:18674] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f41a005518b]
[fv-az99-305:18674] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f41a0034859]
[fv-az99-305:18674] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f41a02bc951]
[fv-az99-305:18674] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f41a02c847c]
[fv-az99-305:18674] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f41a02c84e7]
[fv-az99-305:18674] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f41a02c8799]
[fv-az99-305:18674] [ 7] plumed(+0xf47d)[0x55b563d6247d]
[fv-az99-305:18674] [ 8] plumed(+0x14004)[0x55b563d67004]
[fv-az99-305:18674] [ 9] plumed(+0xf698)[0x55b563d62698]
[fv-az99-305:18674] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f41a00360b3]
[fv-az99-305:18674] [11] plumed(+0xf76e)[0x55b563d6276e]
[fv-az99-305:18674] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  MultithermalSimulations/Liquid/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
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
[fv-az99-305:18704] *** Process received signal ***
[fv-az99-305:18704] Signal: Aborted (6)
[fv-az99-305:18704] Signal code:  (-6)
[fv-az99-305:18704] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ff2af14a210]
[fv-az99-305:18704] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ff2af14a18b]
[fv-az99-305:18704] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ff2af129859]
[fv-az99-305:18704] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ff2af3b1951]
[fv-az99-305:18704] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ff2af3bd47c]
[fv-az99-305:18704] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ff2af3bd4e7]
[fv-az99-305:18704] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7ff2af3bd799]
[fv-az99-305:18704] [ 7] plumed(+0xf47d)[0x55f4bab6e47d]
[fv-az99-305:18704] [ 8] plumed(+0x14004)[0x55f4bab73004]
[fv-az99-305:18704] [ 9] plumed(+0xf698)[0x55f4bab6e698]
[fv-az99-305:18704] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ff2af12b0b3]
[fv-az99-305:18704] [11] plumed(+0xf76e)[0x55f4bab6e76e]
[fv-az99-305:18704] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=350 MIN_TEMP=260 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18705] *** Process received signal ***
[fv-az99-305:18705] Signal: Aborted (6)
[fv-az99-305:18705] Signal code:  (-6)
[fv-az99-305:18705] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fadd66d6210]
[fv-az99-305:18705] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fadd66d618b]
[fv-az99-305:18705] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fadd66b5859]
[fv-az99-305:18705] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fadd693d951]
[fv-az99-305:18705] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fadd694947c]
[fv-az99-305:18705] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fadd69494e7]
[fv-az99-305:18705] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fadd6949799]
[fv-az99-305:18705] [ 7] plumed(+0xf47d)[0x55eb7f4a547d]
[fv-az99-305:18705] [ 8] plumed(+0x14004)[0x55eb7f4aa004]
[fv-az99-305:18705] [ 9] plumed(+0xf698)[0x55eb7f4a5698]
[fv-az99-305:18705] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fadd66b70b3]
[fv-az99-305:18705] [11] plumed(+0xf76e)[0x55eb7f4a576e]
[fv-az99-305:18705] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

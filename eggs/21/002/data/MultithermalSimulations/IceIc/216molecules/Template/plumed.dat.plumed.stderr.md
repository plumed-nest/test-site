**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  MultithermalSimulations/IceIc/216molecules/Template/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
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
[fv-az99-305:18453] *** Process received signal ***
terminate called after throwing an instance of '[fv-az99-305:18453] Signal: Aborted (6)
[fv-az99-305:18453] Signal code:  (-6)
PLMD::Plumed::ExceptionError[fv-az99-305:18453] [ 0] '
/lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb6567dd210]
[fv-az99-305:18453] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb6567dd18b]
[fv-az99-305:18453] [ 2]   what():  /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb6567bc859]
[fv-az99-305:18453] [ 3] 
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=305 MIN_TEMP=260 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
/lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb656a44951]
[fv-az99-305:18453] [ 4] [fv-az99-305:18454] *** Process received signal ***
/lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb656a5047c]
[fv-az99-305:18453] [ 5] [fv-az99-305:18454] Signal: Aborted (6)
[fv-az99-305:18454] Signal code:  (-6)
/lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb656a504e7]
[fv-az99-305:18453] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb656a50799]
[fv-az99-305:18453] [ 7] [fv-az99-305:18454] plumed(+0xf47d)[0x56413fe5547d]
[fv-az99-305:18453] [ 8] plumed(+0x14004)[0x56413fe5a004]
[fv-az99-305:18453] [ 9] plumed(+0xf698)[0x56413fe55698]
[fv-az99-305:18453] [10] [ 0] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb6567be0b3]
[fv-az99-305:18453] [11] plumed(+0xf76e)[0x56413fe5576e]
[fv-az99-305:18453] *** End of error message ***
/lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f3b27c16210]
[fv-az99-305:18454] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f3b27c1618b]
[fv-az99-305:18454] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f3b27bf5859]
[fv-az99-305:18454] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f3b27e7d951]
[fv-az99-305:18454] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f3b27e8947c]
[fv-az99-305:18454] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f3b27e894e7]
[fv-az99-305:18454] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f3b27e89799]
[fv-az99-305:18454] [ 7] plumed(+0xf47d)[0x56264375147d]
[fv-az99-305:18454] [ 8] plumed(+0x14004)[0x562643756004]
[fv-az99-305:18454] [ 9] plumed(+0xf698)[0x562643751698]
[fv-az99-305:18454] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f3b27bf70b3]
[fv-az99-305:18454] [11] plumed(+0xf76e)[0x56264375176e]
[fv-az99-305:18454] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

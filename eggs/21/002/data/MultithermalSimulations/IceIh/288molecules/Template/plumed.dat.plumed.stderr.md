**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  MultithermalSimulations/IceIh/288molecules/Template/plumed.dat   
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
[fv-az99-305:18643] *** Process received signal ***
[fv-az99-305:18643] Signal: Aborted (6)
[fv-az99-305:18643] Signal code:  (-6)
[fv-az99-305:18643] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb916727210]
[fv-az99-305:18643] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb91672718b]
[fv-az99-305:18643] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb916706859]
[fv-az99-305:18643] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb91698e951]
[fv-az99-305:18643] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb91699a47c]
[fv-az99-305:18643] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb91699a4e7]
[fv-az99-305:18643] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb91699a799]
[fv-az99-305:18643] [ 7] plumed(+0xf47d)[0x55c3f7ff047d]
[fv-az99-305:18643] [ 8] plumed(+0x14004)[0x55c3f7ff5004]
[fv-az99-305:18643] [ 9] plumed(+0xf698)[0x55c3f7ff0698]
[fv-az99-305:18643] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb9167080b3]
[fv-az99-305:18643] [11] plumed(+0xf76e)[0x55c3f7ff076e]
[fv-az99-305:18643] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=305 MIN_TEMP=260 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18644] *** Process received signal ***
[fv-az99-305:18644] Signal: Aborted (6)
[fv-az99-305:18644] Signal code:  (-6)
[fv-az99-305:18644] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f209faac210]
[fv-az99-305:18644] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f209faac18b]
[fv-az99-305:18644] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f209fa8b859]
[fv-az99-305:18644] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f209fd13951]
[fv-az99-305:18644] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f209fd1f47c]
[fv-az99-305:18644] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f209fd1f4e7]
[fv-az99-305:18644] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f209fd1f799]
[fv-az99-305:18644] [ 7] plumed(+0xf47d)[0x556ac90ef47d]
[fv-az99-305:18644] [ 8] plumed(+0x14004)[0x556ac90f4004]
[fv-az99-305:18644] [ 9] plumed(+0xf698)[0x556ac90ef698]
[fv-az99-305:18644] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f209fa8d0b3]
[fv-az99-305:18644] [11] plumed(+0xf76e)[0x556ac90ef76e]
[fv-az99-305:18644] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 1 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  MultithermalSimulations/IceIc/216molecules/Template/plumed.start.dat   
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
[fv-az99-305:18484] *** Process received signal ***
[fv-az99-305:18484] Signal: Aborted (6)
[fv-az99-305:18484] Signal code:  (-6)
[fv-az99-305:18484] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f48a869d210]
[fv-az99-305:18484] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f48a869d18b]
[fv-az99-305:18484] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f48a867c859]
[fv-az99-305:18484] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f48a8904951]
[fv-az99-305:18484] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f48a891047c]
[fv-az99-305:18484] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f48a89104e7]
[fv-az99-305:18484] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f48a8910799]
[fv-az99-305:18484] [ 7] plumed(+0xf47d)[0x56213526447d]
[fv-az99-305:18484] [ 8] plumed(+0x14004)[0x562135269004]
[fv-az99-305:18484] [ 9] plumed(+0xf698)[0x562135264698]
[fv-az99-305:18484] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f48a867e0b3]
[fv-az99-305:18484] [11] plumed(+0xf76e)[0x56213526476e]
[fv-az99-305:18484] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=305 MIN_TEMP=260 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18485] *** Process received signal ***
[fv-az99-305:18485] Signal: Aborted (6)
[fv-az99-305:18485] Signal code:  (-6)
[fv-az99-305:18485] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe2d5971210]
[fv-az99-305:18485] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe2d597118b]
[fv-az99-305:18485] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe2d5950859]
[fv-az99-305:18485] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe2d5bd8951]
[fv-az99-305:18485] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe2d5be447c]
[fv-az99-305:18485] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe2d5be44e7]
[fv-az99-305:18485] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fe2d5be4799]
[fv-az99-305:18485] [ 7] plumed(+0xf47d)[0x558f8bee347d]
[fv-az99-305:18485] [ 8] plumed(+0x14004)[0x558f8bee8004]
[fv-az99-305:18485] [ 9] plumed(+0xf698)[0x558f8bee3698]
[fv-az99-305:18485] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe2d59520b3]
[fv-az99-305:18485] [11] plumed(+0xf76e)[0x558f8bee376e]
[fv-az99-305:18485] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

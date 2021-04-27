**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  Crystallization/IceIc/64molecules/Multithermal/plumed.start.dat   
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
[fv-az99-305:18130] *** Process received signal ***
[fv-az99-305:18130] Signal: Aborted (6)
[fv-az99-305:18130] Signal code:  (-6)
[fv-az99-305:18130] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe17e77f210]
[fv-az99-305:18130] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe17e77f18b]
[fv-az99-305:18130] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe17e75e859]
[fv-az99-305:18130] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe17e9e6951]
[fv-az99-305:18130] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe17e9f247c]
[fv-az99-305:18130] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe17e9f24e7]
[fv-az99-305:18130] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fe17e9f2799]
[fv-az99-305:18130] [ 7] plumed(+0xf47d)[0x55a04ca4747d]
[fv-az99-305:18130] [ 8] plumed(+0x14004)[0x55a04ca4c004]
[fv-az99-305:18130] [ 9] plumed(+0xf698)[0x55a04ca47698]
[fv-az99-305:18130] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe17e7600b3]
[fv-az99-305:18130] [11] plumed(+0xf76e)[0x55a04ca4776e]
[fv-az99-305:18130] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=330 MIN_TEMP=300 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18129] *** Process received signal ***
[fv-az99-305:18129] Signal: Aborted (6)
[fv-az99-305:18129] Signal code:  (-6)
[fv-az99-305:18129] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7efdef15b210]
[fv-az99-305:18129] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7efdef15b18b]
[fv-az99-305:18129] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7efdef13a859]
[fv-az99-305:18129] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7efdef3c2951]
[fv-az99-305:18129] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7efdef3ce47c]
[fv-az99-305:18129] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7efdef3ce4e7]
[fv-az99-305:18129] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7efdef3ce799]
[fv-az99-305:18129] [ 7] plumed(+0xf47d)[0x55be3aef147d]
[fv-az99-305:18129] [ 8] plumed(+0x14004)[0x55be3aef6004]
[fv-az99-305:18129] [ 9] plumed(+0xf698)[0x55be3aef1698]
[fv-az99-305:18129] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7efdef13c0b3]
[fv-az99-305:18129] [11] plumed(+0xf76e)[0x55be3aef176e]
[fv-az99-305:18129] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

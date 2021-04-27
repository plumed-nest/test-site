**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  Crystallization/IceIc/96molecules/Multithermal/plumed.start.dat   
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
[fv-az99-305:18190] *** Process received signal ***
[fv-az99-305:18190] Signal: Aborted (6)
[fv-az99-305:18190] Signal code:  (-6)
[fv-az99-305:18190] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fca863dc210]
[fv-az99-305:18190] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fca863dc18b]
[fv-az99-305:18190] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fca863bb859]
[fv-az99-305:18190] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fca86643951]
[fv-az99-305:18190] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fca8664f47c]
[fv-az99-305:18190] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fca8664f4e7]
[fv-az99-305:18190] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fca8664f799]
[fv-az99-305:18190] [ 7] plumed(+0xf47d)[0x55cb234da47d]
[fv-az99-305:18190] [ 8] plumed(+0x14004)[0x55cb234df004]
[fv-az99-305:18190] [ 9] plumed(+0xf698)[0x55cb234da698]
[fv-az99-305:18190] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fca863bd0b3]
[fv-az99-305:18190] [11] plumed(+0xf76e)[0x55cb234da76e]
[fv-az99-305:18190] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=330 MIN_TEMP=300 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18191] *** Process received signal ***
[fv-az99-305:18191] Signal: Aborted (6)
[fv-az99-305:18191] Signal code:  (-6)
[fv-az99-305:18191] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5fde9d7210]
[fv-az99-305:18191] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5fde9d718b]
[fv-az99-305:18191] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5fde9b6859]
[fv-az99-305:18191] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5fdec3e951]
[fv-az99-305:18191] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5fdec4a47c]
[fv-az99-305:18191] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5fdec4a4e7]
[fv-az99-305:18191] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f5fdec4a799]
[fv-az99-305:18191] [ 7] plumed(+0xf47d)[0x5617448ee47d]
[fv-az99-305:18191] [ 8] plumed(+0x14004)[0x5617448f3004]
[fv-az99-305:18191] [ 9] plumed(+0xf698)[0x5617448ee698]
[fv-az99-305:18191] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5fde9b80b3]
[fv-az99-305:18191] [11] plumed(+0xf76e)[0x5617448ee76e]
[fv-az99-305:18191] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 1 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

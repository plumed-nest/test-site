**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  Reweight/Example/NNP/plumed.dat   
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
[fv-az99-305:18767] *** Process received signal ***
[fv-az99-305:18767] Signal: Aborted (6)
[fv-az99-305:18767] Signal code:  (-6)
[fv-az99-305:18767] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb2d512c210]
[fv-az99-305:18767] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb2d512c18b]
[fv-az99-305:18767] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb2d510b859]
[fv-az99-305:18767] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb2d5393951]
[fv-az99-305:18767] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb2d539f47c]
[fv-az99-305:18767] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb2d539f4e7]
[fv-az99-305:18767] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb2d539f799]
[fv-az99-305:18767] [ 7] plumed(+0xf47d)[0x556de63e547d]
[fv-az99-305:18767] [ 8] plumed(+0x14004)[0x556de63ea004]
[fv-az99-305:18767] [ 9] plumed(+0xf698)[0x556de63e5698]
[fv-az99-305:18767] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb2d510d0b3]
[fv-az99-305:18767] [11] plumed(+0xf76e)[0x556de63e576e]
[fv-az99-305:18767] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=330 MIN_TEMP=300 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18768] *** Process received signal ***
[fv-az99-305:18768] Signal: Aborted (6)
[fv-az99-305:18768] Signal code:  (-6)
[fv-az99-305:18768] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f8af149d210]
[fv-az99-305:18768] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f8af149d18b]
[fv-az99-305:18768] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f8af147c859]
[fv-az99-305:18768] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f8af1704951]
[fv-az99-305:18768] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f8af171047c]
[fv-az99-305:18768] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f8af17104e7]
[fv-az99-305:18768] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f8af1710799]
[fv-az99-305:18768] [ 7] plumed(+0xf47d)[0x5651ed12c47d]
[fv-az99-305:18768] [ 8] plumed(+0x14004)[0x5651ed131004]
[fv-az99-305:18768] [ 9] plumed(+0xf698)[0x5651ed12c698]
[fv-az99-305:18768] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f8af147e0b3]
[fv-az99-305:18768] [11] plumed(+0xf76e)[0x5651ed12c76e]
[fv-az99-305:18768] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 1 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

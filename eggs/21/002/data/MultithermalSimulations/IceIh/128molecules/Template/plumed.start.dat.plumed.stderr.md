**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  MultithermalSimulations/IceIh/128molecules/Template/plumed.start.dat   
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
[fv-az99-305:18612] *** Process received signal ***
[fv-az99-305:18612] Signal: Aborted (6)
[fv-az99-305:18612] Signal code:  (-6)
[fv-az99-305:18612] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4a53dc1210]
[fv-az99-305:18612] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4a53dc118b]
[fv-az99-305:18612] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4a53da0859]
[fv-az99-305:18612] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4a54028951]
[fv-az99-305:18612] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f4a5403447c]
[fv-az99-305:18612] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f4a540344e7]
[fv-az99-305:18612] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4a54034799]
[fv-az99-305:18612] [ 7] plumed(+0xf47d)[0x56105f16c47d]
[fv-az99-305:18612] [ 8] plumed(+0x14004)[0x56105f171004]
[fv-az99-305:18612] [ 9] plumed(+0xf698)[0x56105f16c698]
[fv-az99-305:18612] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4a53da20b3]
[fv-az99-305:18612] [11] plumed(+0xf76e)[0x56105f16c76e]
[fv-az99-305:18612] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=225 MIN_TEMP=100 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18613] *** Process received signal ***
[fv-az99-305:18613] Signal: Aborted (6)
[fv-az99-305:18613] Signal code:  (-6)
[fv-az99-305:18613] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f85bac24210]
[fv-az99-305:18613] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f85bac2418b]
[fv-az99-305:18613] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f85bac03859]
[fv-az99-305:18613] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f85bae8b951]
[fv-az99-305:18613] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f85bae9747c]
[fv-az99-305:18613] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f85bae974e7]
[fv-az99-305:18613] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f85bae97799]
[fv-az99-305:18613] [ 7] plumed(+0xf47d)[0x55c35691947d]
[fv-az99-305:18613] [ 8] plumed(+0x14004)[0x55c35691e004]
[fv-az99-305:18613] [ 9] plumed(+0xf698)[0x55c356919698]
[fv-az99-305:18613] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f85bac050b3]
[fv-az99-305:18613] [11] plumed(+0xf76e)[0x55c35691976e]
[fv-az99-305:18613] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

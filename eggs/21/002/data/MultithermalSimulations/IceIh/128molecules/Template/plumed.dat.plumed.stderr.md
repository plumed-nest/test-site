**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  MultithermalSimulations/IceIh/128molecules/Template/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
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
[fv-az99-305:18582] *** Process received signal ***
[fv-az99-305:18582] Signal: Aborted (6)
[fv-az99-305:18582] Signal code:  (-6)
[fv-az99-305:18582] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f1542674210]
[fv-az99-305:18582] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f154267418b]
[fv-az99-305:18582] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f1542653859]
[fv-az99-305:18582] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f15428db951]
[fv-az99-305:18582] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f15428e747c]
[fv-az99-305:18582] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f15428e74e7]
[fv-az99-305:18582] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f15428e7799]
[fv-az99-305:18582] [ 7] plumed(+0xf47d)[0x5640f5b4947d]
[fv-az99-305:18582] [ 8] plumed(+0x14004)[0x5640f5b4e004]
[fv-az99-305:18582] [ 9] plumed(+0xf698)[0x5640f5b49698]
[fv-az99-305:18582] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f15426550b3]
[fv-az99-305:18582] [11] plumed(+0xf76e)[0x5640f5b4976e]
[fv-az99-305:18582] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=225 MIN_TEMP=100 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18583] *** Process received signal ***
[fv-az99-305:18583] Signal: Aborted (6)
[fv-az99-305:18583] Signal code:  (-6)
[fv-az99-305:18583] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f41a6c7d210]
[fv-az99-305:18583] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f41a6c7d18b]
[fv-az99-305:18583] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f41a6c5c859]
[fv-az99-305:18583] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f41a6ee4951]
[fv-az99-305:18583] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f41a6ef047c]
[fv-az99-305:18583] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f41a6ef04e7]
[fv-az99-305:18583] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f41a6ef0799]
[fv-az99-305:18583] [ 7] plumed(+0xf47d)[0x55bd0ae8447d]
[fv-az99-305:18583] [ 8] plumed(+0x14004)[0x55bd0ae89004]
[fv-az99-305:18583] [ 9] plumed(+0xf698)[0x55bd0ae84698]
[fv-az99-305:18583] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f41a6c5e0b3]
[fv-az99-305:18583] [11] plumed(+0xf76e)[0x55bd0ae8476e]
[fv-az99-305:18583] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

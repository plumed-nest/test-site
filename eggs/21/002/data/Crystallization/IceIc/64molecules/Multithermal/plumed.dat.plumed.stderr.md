**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  Crystallization/IceIc/64molecules/Multithermal/plumed.dat   
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
[fv-az99-305:18100] *** Process received signal ***
[fv-az99-305:18100] Signal: Aborted (6)
[fv-az99-305:18100] Signal code:  (-6)
[fv-az99-305:18100] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4335f8f210]
[fv-az99-305:18100] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4335f8f18b]
[fv-az99-305:18100] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4335f6e859]
[fv-az99-305:18100] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f43361f6951]
[fv-az99-305:18100] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f433620247c]
[fv-az99-305:18100] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f43362024e7]
[fv-az99-305:18100] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4336202799]
[fv-az99-305:18100] [ 7] plumed(+0xf47d)[0x55c69fe1e47d]
[fv-az99-305:18100] [ 8] plumed(+0x14004)[0x55c69fe23004]
[fv-az99-305:18100] [ 9] plumed(+0xf698)[0x55c69fe1e698]
[fv-az99-305:18100] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4335f700b3]
[fv-az99-305:18100] [11] plumed(+0xf76e)[0x55c69fe1e76e]
[fv-az99-305:18100] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=330 MIN_TEMP=300 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18099] *** Process received signal ***
[fv-az99-305:18099] Signal: Aborted (6)
[fv-az99-305:18099] Signal code:  (-6)
[fv-az99-305:18099] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd66b855210]
[fv-az99-305:18099] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd66b85518b]
[fv-az99-305:18099] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd66b834859]
[fv-az99-305:18099] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd66babc951]
[fv-az99-305:18099] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd66bac847c]
[fv-az99-305:18099] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd66bac84e7]
[fv-az99-305:18099] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd66bac8799]
[fv-az99-305:18099] [ 7] plumed(+0xf47d)[0x55b09f30147d]
[fv-az99-305:18099] [ 8] plumed(+0x14004)[0x55b09f306004]
[fv-az99-305:18099] [ 9] plumed(+0xf698)[0x55b09f301698]
[fv-az99-305:18099] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd66b8360b3]
[fv-az99-305:18099] [11] plumed(+0xf76e)[0x55b09f30176e]
[fv-az99-305:18099] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 1 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

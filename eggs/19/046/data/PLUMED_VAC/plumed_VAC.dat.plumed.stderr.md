**Project ID:** [plumID:19.046]({{ '/' | absolute_url }}eggs/19/046/)  
Stderr for source:  PLUMED_VAC/plumed_VAC.dat   
(download [zipped raw stdout](plumed_VAC.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: TICA ARG=Prot_norm,wBpock_norm,ab_t,lig_OW_large_norm EIGEN_NUMBERS=4 LAGGED_TIME=150000 TAU_NUMBER=5000 STEP_SIZE=0.5 LOGWEIGHTS=rw
Maybe a missing space or a typo?
[fv-az99-305:37101] *** Process received signal ***
[fv-az99-305:37101] Signal: Aborted (6)
[fv-az99-305:37101] Signal code:  (-6)
[fv-az99-305:37101] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7feb7ab15210]
[fv-az99-305:37101] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7feb7ab1518b]
[fv-az99-305:37101] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7feb7aaf4859]
[fv-az99-305:37101] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7feb7ad7c951]
[fv-az99-305:37101] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7feb7ad8847c]
[fv-az99-305:37101] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7feb7ad884e7]
[fv-az99-305:37101] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7feb7ad88799]
[fv-az99-305:37101] [ 7] plumed(+0xf47d)[0x5654656a047d]
[fv-az99-305:37101] [ 8] plumed(+0x14004)[0x5654656a5004]
[fv-az99-305:37101] [ 9] plumed(+0xf698)[0x5654656a0698]
[fv-az99-305:37101] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7feb7aaf60b3]
[fv-az99-305:37101] [11] plumed(+0xf76e)[0x5654656a076e]
[fv-az99-305:37101] *** End of error message ***
</pre>
{% endraw %}

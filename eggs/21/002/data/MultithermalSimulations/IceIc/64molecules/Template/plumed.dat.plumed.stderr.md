**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
Stderr for source:  MultithermalSimulations/IceIc/64molecules/Template/plumed.dat   
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
[fv-az99-305:18519] *** Process received signal ***
[fv-az99-305:18519] Signal: Aborted (6)
[fv-az99-305:18519] Signal code:  (-6)
[fv-az99-305:18519] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f468f86c210]
[fv-az99-305:18519] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f468f86c18b]
[fv-az99-305:18519] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f468f84b859]
[fv-az99-305:18519] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f468fad3951]
[fv-az99-305:18519] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f468fadf47c]
[fv-az99-305:18519] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f468fadf4e7]
[fv-az99-305:18519] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f468fadf799]
[fv-az99-305:18519] [ 7] plumed(+0xf47d)[0x5653a9c9247d]
[fv-az99-305:18519] [ 8] plumed(+0x14004)[0x5653a9c97004]
[fv-az99-305:18519] [ 9] plumed(+0xf698)[0x5653a9c92698]
[fv-az99-305:18519] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f468f84d0b3]
[fv-az99-305:18519] [11] plumed(+0xf76e)[0x5653a9c9276e]
[fv-az99-305:18519] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=energy,vol TEMP=225 MIN_TEMP=100 MAX_TEMP=350 PRESSURE=0.06022140857 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857
Maybe a missing space or a typo?
[fv-az99-305:18520] *** Process received signal ***
[fv-az99-305:18520] Signal: Aborted (6)
[fv-az99-305:18520] Signal code:  (-6)
[fv-az99-305:18520] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb4520f3210]
[fv-az99-305:18520] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb4520f318b]
[fv-az99-305:18520] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb4520d2859]
[fv-az99-305:18520] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb45235a951]
[fv-az99-305:18520] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb45236647c]
[fv-az99-305:18520] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb4523664e7]
[fv-az99-305:18520] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb452366799]
[fv-az99-305:18520] [ 7] plumed(+0xf47d)[0x565173dca47d]
[fv-az99-305:18520] [ 8] plumed(+0x14004)[0x565173dcf004]
[fv-az99-305:18520] [ 9] plumed(+0xf698)[0x565173dca698]
[fv-az99-305:18520] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb4520d40b3]
[fv-az99-305:18520] [11] plumed(+0xf76e)[0x565173dca76e]
[fv-az99-305:18520] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpiexec noticed that process rank 0 with PID 0 on node fv-az99-305 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

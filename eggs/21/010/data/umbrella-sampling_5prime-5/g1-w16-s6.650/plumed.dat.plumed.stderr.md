**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w16-s6.650/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az99-305:15776] *** Process received signal ***
[fv-az99-305:15776] Signal: Aborted (6)
[fv-az99-305:15776] Signal code:  (-6)
[fv-az99-305:15776] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa5743ae210]
[fv-az99-305:15776] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa5743ae18b]
[fv-az99-305:15776] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa57438d859]
[fv-az99-305:15776] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa574615951]
[fv-az99-305:15776] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa57462147c]
[fv-az99-305:15776] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa5746214e7]
[fv-az99-305:15776] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fa574621799]
[fv-az99-305:15776] [ 7] plumed(+0xf47d)[0x56353143e47d]
[fv-az99-305:15776] [ 8] plumed(+0x14004)[0x563531443004]
[fv-az99-305:15776] [ 9] plumed(+0xf698)[0x56353143e698]
[fv-az99-305:15776] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa57438f0b3]
[fv-az99-305:15776] [11] plumed(+0xf76e)[0x56353143e76e]
[fv-az99-305:15776] *** End of error message ***
</pre>
{% endraw %}

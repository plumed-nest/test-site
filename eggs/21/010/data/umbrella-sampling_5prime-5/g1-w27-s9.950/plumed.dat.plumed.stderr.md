**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w27-s9.950/plumed.dat   
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
[fv-az99-305:16070] *** Process received signal ***
[fv-az99-305:16070] Signal: Aborted (6)
[fv-az99-305:16070] Signal code:  (-6)
[fv-az99-305:16070] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fdfe0d8a210]
[fv-az99-305:16070] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fdfe0d8a18b]
[fv-az99-305:16070] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fdfe0d69859]
[fv-az99-305:16070] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fdfe0ff1951]
[fv-az99-305:16070] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fdfe0ffd47c]
[fv-az99-305:16070] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fdfe0ffd4e7]
[fv-az99-305:16070] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fdfe0ffd799]
[fv-az99-305:16070] [ 7] plumed(+0xf47d)[0x55f266d9847d]
[fv-az99-305:16070] [ 8] plumed(+0x14004)[0x55f266d9d004]
[fv-az99-305:16070] [ 9] plumed(+0xf698)[0x55f266d98698]
[fv-az99-305:16070] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fdfe0d6b0b3]
[fv-az99-305:16070] [11] plumed(+0xf76e)[0x55f266d9876e]
[fv-az99-305:16070] *** End of error message ***
</pre>
{% endraw %}

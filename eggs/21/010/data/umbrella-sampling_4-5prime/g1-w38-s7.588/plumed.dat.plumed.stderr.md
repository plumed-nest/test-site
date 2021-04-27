**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w38-s7.588/plumed.dat   
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
[fv-az99-305:13545] *** Process received signal ***
[fv-az99-305:13545] Signal: Aborted (6)
[fv-az99-305:13545] Signal code:  (-6)
[fv-az99-305:13545] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7efe0a7ed210]
[fv-az99-305:13545] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7efe0a7ed18b]
[fv-az99-305:13545] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7efe0a7cc859]
[fv-az99-305:13545] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7efe0aa54951]
[fv-az99-305:13545] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7efe0aa6047c]
[fv-az99-305:13545] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7efe0aa604e7]
[fv-az99-305:13545] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7efe0aa60799]
[fv-az99-305:13545] [ 7] plumed(+0xf47d)[0x562c798e647d]
[fv-az99-305:13545] [ 8] plumed(+0x14004)[0x562c798eb004]
[fv-az99-305:13545] [ 9] plumed(+0xf698)[0x562c798e6698]
[fv-az99-305:13545] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7efe0a7ce0b3]
[fv-az99-305:13545] [11] plumed(+0xf76e)[0x562c798e676e]
[fv-az99-305:13545] *** End of error message ***
</pre>
{% endraw %}

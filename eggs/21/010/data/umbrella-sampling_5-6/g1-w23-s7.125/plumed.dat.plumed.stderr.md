**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w23-s7.125/plumed.dat   
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
[fv-az99-305:14745] *** Process received signal ***
[fv-az99-305:14745] Signal: Aborted (6)
[fv-az99-305:14745] Signal code:  (-6)
[fv-az99-305:14745] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f8755b3a210]
[fv-az99-305:14745] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f8755b3a18b]
[fv-az99-305:14745] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f8755b19859]
[fv-az99-305:14745] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f8755da1951]
[fv-az99-305:14745] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f8755dad47c]
[fv-az99-305:14745] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f8755dad4e7]
[fv-az99-305:14745] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f8755dad799]
[fv-az99-305:14745] [ 7] plumed(+0xf47d)[0x55d3a485c47d]
[fv-az99-305:14745] [ 8] plumed(+0x14004)[0x55d3a4861004]
[fv-az99-305:14745] [ 9] plumed(+0xf698)[0x55d3a485c698]
[fv-az99-305:14745] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f8755b1b0b3]
[fv-az99-305:14745] [11] plumed(+0xf76e)[0x55d3a485c76e]
[fv-az99-305:14745] *** End of error message ***
</pre>
{% endraw %}

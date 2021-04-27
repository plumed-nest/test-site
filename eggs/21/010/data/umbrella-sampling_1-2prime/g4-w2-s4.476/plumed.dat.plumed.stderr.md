**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g4-w2-s4.476/plumed.dat   
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
[fv-az99-305:09869] *** Process received signal ***
[fv-az99-305:09869] Signal: Aborted (6)
[fv-az99-305:09869] Signal code:  (-6)
[fv-az99-305:09869] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7ee764e210]
[fv-az99-305:09869] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7ee764e18b]
[fv-az99-305:09869] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7ee762d859]
[fv-az99-305:09869] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7ee78b5951]
[fv-az99-305:09869] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7ee78c147c]
[fv-az99-305:09869] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7ee78c14e7]
[fv-az99-305:09869] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f7ee78c1799]
[fv-az99-305:09869] [ 7] plumed(+0xf47d)[0x55655506c47d]
[fv-az99-305:09869] [ 8] plumed(+0x14004)[0x556555071004]
[fv-az99-305:09869] [ 9] plumed(+0xf698)[0x55655506c698]
[fv-az99-305:09869] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7ee762f0b3]
[fv-az99-305:09869] [11] plumed(+0xf76e)[0x55655506c76e]
[fv-az99-305:09869] *** End of error message ***
</pre>
{% endraw %}

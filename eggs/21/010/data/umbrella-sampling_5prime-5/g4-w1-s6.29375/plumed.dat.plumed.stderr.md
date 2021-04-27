**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g4-w1-s6.29375/plumed.dat   
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
[fv-az99-305:16413] *** Process received signal ***
[fv-az99-305:16413] Signal: Aborted (6)
[fv-az99-305:16413] Signal code:  (-6)
[fv-az99-305:16413] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f1668b29210]
[fv-az99-305:16413] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f1668b2918b]
[fv-az99-305:16413] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f1668b08859]
[fv-az99-305:16413] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f1668d90951]
[fv-az99-305:16413] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f1668d9c47c]
[fv-az99-305:16413] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f1668d9c4e7]
[fv-az99-305:16413] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f1668d9c799]
[fv-az99-305:16413] [ 7] plumed(+0xf47d)[0x56288875447d]
[fv-az99-305:16413] [ 8] plumed(+0x14004)[0x562888759004]
[fv-az99-305:16413] [ 9] plumed(+0xf698)[0x562888754698]
[fv-az99-305:16413] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f1668b0a0b3]
[fv-az99-305:16413] [11] plumed(+0xf76e)[0x56288875476e]
[fv-az99-305:16413] *** End of error message ***
</pre>
{% endraw %}

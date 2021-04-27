**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g2-w1-s4.44/plumed.dat   
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
[fv-az99-305:09772] *** Process received signal ***
[fv-az99-305:09772] Signal: Aborted (6)
[fv-az99-305:09772] Signal code:  (-6)
[fv-az99-305:09772] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f244d134210]
[fv-az99-305:09772] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f244d13418b]
[fv-az99-305:09772] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f244d113859]
[fv-az99-305:09772] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f244d39b951]
[fv-az99-305:09772] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f244d3a747c]
[fv-az99-305:09772] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f244d3a74e7]
[fv-az99-305:09772] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f244d3a7799]
[fv-az99-305:09772] [ 7] plumed(+0xf47d)[0x5568ffba447d]
[fv-az99-305:09772] [ 8] plumed(+0x14004)[0x5568ffba9004]
[fv-az99-305:09772] [ 9] plumed(+0xf698)[0x5568ffba4698]
[fv-az99-305:09772] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f244d1150b3]
[fv-az99-305:09772] [11] plumed(+0xf76e)[0x5568ffba476e]
[fv-az99-305:09772] *** End of error message ***
</pre>
{% endraw %}

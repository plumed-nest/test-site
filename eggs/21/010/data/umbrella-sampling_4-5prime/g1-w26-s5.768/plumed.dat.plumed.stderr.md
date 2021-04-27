**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w26-s5.768/plumed.dat   
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
[fv-az99-305:13227] *** Process received signal ***
[fv-az99-305:13227] Signal: Aborted (6)
[fv-az99-305:13227] Signal code:  (-6)
[fv-az99-305:13227] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa5c4e45210]
[fv-az99-305:13227] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa5c4e4518b]
[fv-az99-305:13227] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa5c4e24859]
[fv-az99-305:13227] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa5c50ac951]
[fv-az99-305:13227] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa5c50b847c]
[fv-az99-305:13227] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa5c50b84e7]
[fv-az99-305:13227] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fa5c50b8799]
[fv-az99-305:13227] [ 7] plumed(+0xf47d)[0x558dca7ca47d]
[fv-az99-305:13227] [ 8] plumed(+0x14004)[0x558dca7cf004]
[fv-az99-305:13227] [ 9] plumed(+0xf698)[0x558dca7ca698]
[fv-az99-305:13227] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa5c4e260b3]
[fv-az99-305:13227] [11] plumed(+0xf76e)[0x558dca7ca76e]
[fv-az99-305:13227] *** End of error message ***
</pre>
{% endraw %}

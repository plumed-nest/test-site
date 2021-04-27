**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w12-s5.450/plumed.dat   
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
[fv-az99-305:15675] *** Process received signal ***
[fv-az99-305:15675] Signal: Aborted (6)
[fv-az99-305:15675] Signal code:  (-6)
[fv-az99-305:15675] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f131f464210]
[fv-az99-305:15675] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f131f46418b]
[fv-az99-305:15675] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f131f443859]
[fv-az99-305:15675] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f131f6cb951]
[fv-az99-305:15675] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f131f6d747c]
[fv-az99-305:15675] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f131f6d74e7]
[fv-az99-305:15675] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f131f6d7799]
[fv-az99-305:15675] [ 7] plumed(+0xf47d)[0x56355da8547d]
[fv-az99-305:15675] [ 8] plumed(+0x14004)[0x56355da8a004]
[fv-az99-305:15675] [ 9] plumed(+0xf698)[0x56355da85698]
[fv-az99-305:15675] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f131f4450b3]
[fv-az99-305:15675] [11] plumed(+0xf76e)[0x56355da8576e]
[fv-az99-305:15675] *** End of error message ***
</pre>
{% endraw %}

**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g6-w1-s6.208/plumed.dat   
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
[fv-az99-305:15528] *** Process received signal ***
[fv-az99-305:15528] Signal: Aborted (6)
[fv-az99-305:15528] Signal code:  (-6)
[fv-az99-305:15528] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd6753e7210]
[fv-az99-305:15528] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd6753e718b]
[fv-az99-305:15528] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd6753c6859]
[fv-az99-305:15528] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd67564e951]
[fv-az99-305:15528] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd67565a47c]
[fv-az99-305:15528] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd67565a4e7]
[fv-az99-305:15528] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd67565a799]
[fv-az99-305:15528] [ 7] plumed(+0xf47d)[0x55fb86b6c47d]
[fv-az99-305:15528] [ 8] plumed(+0x14004)[0x55fb86b71004]
[fv-az99-305:15528] [ 9] plumed(+0xf698)[0x55fb86b6c698]
[fv-az99-305:15528] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd6753c80b3]
[fv-az99-305:15528] [11] plumed(+0xf76e)[0x55fb86b6c76e]
[fv-az99-305:15528] *** End of error message ***
</pre>
{% endraw %}

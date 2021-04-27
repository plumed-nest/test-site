**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g2-w2-s6.275/plumed.dat   
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
[fv-az99-305:16364] *** Process received signal ***
[fv-az99-305:16364] Signal: Aborted (6)
[fv-az99-305:16364] Signal code:  (-6)
[fv-az99-305:16364] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb1b23a1210]
[fv-az99-305:16364] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb1b23a118b]
[fv-az99-305:16364] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb1b2380859]
[fv-az99-305:16364] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb1b2608951]
[fv-az99-305:16364] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb1b261447c]
[fv-az99-305:16364] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb1b26144e7]
[fv-az99-305:16364] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb1b2614799]
[fv-az99-305:16364] [ 7] plumed(+0xf47d)[0x55f8d0f9a47d]
[fv-az99-305:16364] [ 8] plumed(+0x14004)[0x55f8d0f9f004]
[fv-az99-305:16364] [ 9] plumed(+0xf698)[0x55f8d0f9a698]
[fv-az99-305:16364] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb1b23820b3]
[fv-az99-305:16364] [11] plumed(+0xf76e)[0x55f8d0f9a76e]
[fv-az99-305:16364] *** End of error message ***
</pre>
{% endraw %}

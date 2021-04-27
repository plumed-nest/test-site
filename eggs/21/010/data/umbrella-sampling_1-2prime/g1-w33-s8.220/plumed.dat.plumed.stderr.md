**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w33-s8.220/plumed.dat   
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
[fv-az99-305:09180] *** Process received signal ***
[fv-az99-305:09180] Signal: Aborted (6)
[fv-az99-305:09180] Signal code:  (-6)
[fv-az99-305:09180] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f192b1fe210]
[fv-az99-305:09180] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f192b1fe18b]
[fv-az99-305:09180] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f192b1dd859]
[fv-az99-305:09180] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f192b465951]
[fv-az99-305:09180] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f192b47147c]
[fv-az99-305:09180] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f192b4714e7]
[fv-az99-305:09180] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f192b471799]
[fv-az99-305:09180] [ 7] plumed(+0xf47d)[0x5632aca1a47d]
[fv-az99-305:09180] [ 8] plumed(+0x14004)[0x5632aca1f004]
[fv-az99-305:09180] [ 9] plumed(+0xf698)[0x5632aca1a698]
[fv-az99-305:09180] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f192b1df0b3]
[fv-az99-305:09180] [11] plumed(+0xf76e)[0x5632aca1a76e]
[fv-az99-305:09180] *** End of error message ***
</pre>
{% endraw %}

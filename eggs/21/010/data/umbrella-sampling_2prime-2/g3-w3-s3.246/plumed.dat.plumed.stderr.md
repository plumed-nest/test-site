**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g3-w3-s3.246/plumed.dat   
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
[fv-az99-305:11553] *** Process received signal ***
[fv-az99-305:11553] Signal: Aborted (6)
[fv-az99-305:11553] Signal code:  (-6)
[fv-az99-305:11553] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f400b925210]
[fv-az99-305:11553] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f400b92518b]
[fv-az99-305:11553] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f400b904859]
[fv-az99-305:11553] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f400bb8c951]
[fv-az99-305:11553] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f400bb9847c]
[fv-az99-305:11553] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f400bb984e7]
[fv-az99-305:11553] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f400bb98799]
[fv-az99-305:11553] [ 7] plumed(+0xf47d)[0x55a698a8f47d]
[fv-az99-305:11553] [ 8] plumed(+0x14004)[0x55a698a94004]
[fv-az99-305:11553] [ 9] plumed(+0xf698)[0x55a698a8f698]
[fv-az99-305:11553] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f400b9060b3]
[fv-az99-305:11553] [11] plumed(+0xf76e)[0x55a698a8f76e]
[fv-az99-305:11553] *** End of error message ***
</pre>
{% endraw %}

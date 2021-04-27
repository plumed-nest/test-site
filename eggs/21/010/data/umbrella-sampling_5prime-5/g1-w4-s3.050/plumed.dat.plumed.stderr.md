**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w4-s3.050/plumed.dat   
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
[fv-az99-305:16192] *** Process received signal ***
[fv-az99-305:16192] Signal: Aborted (6)
[fv-az99-305:16192] Signal code:  (-6)
[fv-az99-305:16192] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fdd3a916210]
[fv-az99-305:16192] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fdd3a91618b]
[fv-az99-305:16192] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fdd3a8f5859]
[fv-az99-305:16192] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fdd3ab7d951]
[fv-az99-305:16192] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fdd3ab8947c]
[fv-az99-305:16192] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fdd3ab894e7]
[fv-az99-305:16192] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fdd3ab89799]
[fv-az99-305:16192] [ 7] plumed(+0xf47d)[0x557b09fe547d]
[fv-az99-305:16192] [ 8] plumed(+0x14004)[0x557b09fea004]
[fv-az99-305:16192] [ 9] plumed(+0xf698)[0x557b09fe5698]
[fv-az99-305:16192] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fdd3a8f70b3]
[fv-az99-305:16192] [11] plumed(+0xf76e)[0x557b09fe576e]
[fv-az99-305:16192] *** End of error message ***
</pre>
{% endraw %}
